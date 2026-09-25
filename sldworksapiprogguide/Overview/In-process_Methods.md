<!-- source: sldworksapiprogguide/Overview/In-process_Methods.htm -->

# SOLIDWORKS API Help

# In-process Methods

The SOLIDWORKS API provides two types of methods for interfaces that
get or set arrays:

* in-process
* global

In-process methods typically begin with the letter I and get or set
pointers to arrays that only [unmanaged
C++ applications](Unmanaged_CPP_and_CPP_CLI_Code_Differences.htm) can handle. Global methods (i.e.,
similarly named methods that do not begin with the letter I) are useful both inside a process and across processes and return
predictable results for all of the SOLIDWORKS supported languages.

For example, IView
contains:

* IView::IGetCThreads
  (in-process)
* IView::GetCThreads
   (global)

These methods perform similar work in different languages.

| For... | IView::IGetCThreads gets... | IView::GetCThreads gets... |
| --- | --- | --- |
| VBA, VB.NET, C#, and C++/CLI (also called managed C++) | a CThread | a VARIANT array of CThreads |
| Unmanaged C++ | an array of CThreads | a pointer to a CThread |

In general:

* For VBA, VB.NET, C#, and C++/CLI (also called managed
  C++), in-process methods get or set a strongly typed object, and global
  methods get or set a VARIANT array.
* For unmanaged C++, in-process methods get or set a pointer
  to an array of Dispatch objects, and global methods get or set a pointer to
  a Dispatch object.

The following unmanaged C++ code example uses the flag, useInProcessMethod,
to switch between the in-process method, IView::IGetCThreads,
and the global method, IView::GetCThreads:

STDMETHODIMP CCTDemo::ToolbarCallback0(void)

{

            CComPtr<IModelDoc2>
swModel;

            iSwApp->get\_IActiveDoc2(&swModel);

            CComQIPtr<IDrawingDoc>
swDraw = swModel;

            if
(swDraw)

            {

                  CComPtr<IView>
viewSheet;

                  swDraw->IGetFirstView(&viewSheet);

                  CComPtr<IView>
viewFirst;

                  viewSheet->IGetNextView(&viewFirst);

                  if
(viewFirst)

                  {

                        bool
useInProcessMethod = false;

                        ///Using
IGetCThreads

                        if (useInProcessMethod)

                        {

                              long
count;

                              viewFirst->GetCThreadCount(&count);

                              if
(count > 0)

                              {

                                    CString
msg;

                                    msg.Format(\_T("Number
of threads:  %d"),
count);

                                    long
res0;

                                    iSwApp->SendMsgToUser2(CComBSTR(msg),0,0,&res0);

                                    ICThread\*\*
rawThreadArray = new ICThread\*[count];

                                    viewFirst->IGetCThreads(count, rawThreadArray);

                                    CComPtr<INote>
threadCalloutNote;

                                    rawThreadArray[0]->get\_ThreadCallout(&threadCalloutNote);

                                    if
(threadCalloutNote)

                                    {

                                          CComBSTR
noteText;

                                          threadCalloutNote->GetText(&noteText);

                                          CComBSTR
msg(\_T("Cosmetic thread callout text: "));

                                          if
(noteText != NULL)

                                                msg.Append(noteText);

                                          long
res1;

                                          iSwApp->SendMsgToUser2(CComBSTR(msg),0,0,&res1);

                                    }

                                    //Be
sure to release your resources when you are finished.

                                    for
(int arrayIndex = 0; arrayIndex != count; ++arrayIndex)

                                          rawThreadArray[arrayIndex]->Release();

                                    delete[]
rawThreadArray;

                              }

                              else

                              {

                                    long
res2;

                                    iSwApp->SendMsgToUser2(CComBSTR(\_T("No
threads in drawing view.")),0,0,&res2);

                              }

                        }

                        ///Using GetCThreads

                        ///Note
the use of SafeDISPATCHArray. This is a VARIANT helper class

                        ///that
was defined in a template class.

                        else

                        {

                              long
count;

                              viewFirst->GetCThreadCount(&count);

                              if
(count > 0)

                              {

                                    VARIANT
vThreads;

                                    VariantInit(&vThreads);

                                    viewFirst->GetCThreads(&vThreads);

                                    SafeDISPATCHArray
variantThreadArray(&vThreads);

                                    CComQIPtr<ICThread>
swThread = variantThreadArray[0];

                                    CComPtr<INote>
threadCalloutNote;

                                    swThread->get\_ThreadCallout(&threadCalloutNote);

                                    if
(threadCalloutNote)

                                    {

                                          CComBSTR
noteText;

                                          threadCalloutNote->GetText(&noteText);

                                          CComBSTR
msg(\_T("Cosmetic thread callout text: "));

                                          if
(noteText != NULL)

                                                msg.Append(noteText);

                                          long
res1;

                                          iSwApp->SendMsgToUser2(CComBSTR(msg),0,0,&res1);

                                    }

                                    //Be
sure to release your resources when you are finished.

                                    for
(int arrayIndex = 0; arrayIndex != count; ++arrayIndex)

                                          variantThreadArray[arrayIndex]->Release();

                              }

                              else

                              {

                                    long
res2;

                                    iSwApp->SendMsgToUser2(CComBSTR(\_T("No
threads in drawing view.")),0,0,&res2);

                              }

                        }

                  }

                  else

                  {

                        long
res3;

                        iSwApp->SendMsgToUser2(CComBSTR(\_T("No
drawing view.")),0,0,&res3);

                  }

            }

            else

            {

                  long
res4;

                  iSwApp->SendMsgToUser2(CComBSTR(\_T("No
drawing.")),0,0,&res4);

            }

      return
S\_OK;

}

A VBA programmer might hope that IView::IGetCThreads returns an array. But
this in-process method returns an array only for unmanaged C++. For
VBA, the in-process method returns one strongly typed object, CThread. For
example:

Dim instance As IView

Dim numCThread As Integer

Dim value As CThread

value = instance.IGetCThreads(numCThread)

To reliably obtain the complete array of CThreads, a VBA programmer
(or C# or C++/CLI programmer) should always use the global method
(e.g., IView::GetCThreads). For VBA, IView::GetCThreads returns a VARIANT array of CThreads.  For
example:

Option Explicit

Dim instance As IView

Dim vObj As Variant

Dim CurrCT As SldWorks.Annotation

Dim value As Variant

Sub main()

> Set swApp = Application.SldWorks
>
> Set swModel = swApp.GetFirstDocument
>
> Set instance = swModel.ActiveView
>
> value = instance.GetCThreads
>
> If Not value Is Nothing Then
>
>         For
> i = 0 to UBound(value)
>
>             Set
> CurrCT = value(i)
>
>             Debug.Print
> CurrCT.GetName
>
>         Next
> i
>
> End If

End Sub

For more information about using smart pointers with container classes, see
[STL Container Classes and Smart Pointers](STL_Container_Classes_and_Smart_Pointers.htm).