<!-- source: sldworksapiprogguide/Overview/Return_Values.htm -->

# SOLIDWORKS API Help

# Return Values

If you are using unmanaged C++ COM, the SOLIDWORKS API function always
returns an HRESULT. Any additional return values should be passed by reference
as arguments.

SOLIDWORKS uses HRESULT return values to indicate that the code was
called successfully. It is not meant as an indication that your call achieved
its objective. For example, calling IBody2::IGetFirstFace
will have an HRESULT return value of S\_OK if the code for IBody2::IGetFirstFace
was called successfully. It does not mean that the code succeeded in finding
the first face. In this case, you should check the LPFACE2 return value
for a NULL condition.

## Object Return Values

If an API method returns an object, it is always a good idea to verify
that the object returned is not NULL. This type of error checking is good
programming practice and avoids crashes in your code for unexpected conditions.
For example:

// In unmanaged C++ (COM)

LPFACE m\_Face = NULL;

HRESULT hres = m\_PartDoc->IBodyObject(&m\_Body); //
Get body object from the part

if (m\_Body == NULL) return;

hres = m\_Body->IGetFirstFace(&m\_Face);  //
Get first face object from the body

while (m\_Face != NULL)     //
While faces exist, traverse them

{

double theFaceArea = 0.0;

hres = m\_Face->GetArea(&theFaceArea);  //
Sample use of face object pointer

LPENTITY m\_Entity = NULL;    //
Obtain pointer to Entity object

hres = m\_Face->QueryInterface(
IID\_IEntity, (LPVOID\*)&m\_Entity);

if (m\_Entity != NULL)

{

VARIANT\_BOOL boolres = FALSE;

hres = m\_Entity->Select(TRUE,&boolres); //
Sample use of entity object pointer

m\_Entity->Release();    //
Release Entity object pointer

}

LPFACE pnextFace = NULL;

m\_Face->IGetNextFace(&pnextFace);   //
Get the next face object

m\_Face->Release();     //
Release previous object pointer

m\_Face= pnextFace;

}        //
End while faces exist

m\_PartDoc->Release();     //
Release all pointers when done

m\_Body->Release();     //
Good idea to check for NULL if not certain

// In unmanaged C++ (Dispatch)

LPDISPATCH bodyDisp = m\_PartDoc.Body();  //
Get body object from the part

if (bodyDisp == NULL) return;

IBody m\_Body(bodyDisp);

LPDISPATCH faceDisp = m\_Body.GetFirstFace(); //
Get Dispatch pointer to first face

while (faceDisp)      //
While faces exist, traverse them

{

IFace m\_Face(faceDisp);    //
Get the Face member

double theFaceArea = m\_Face.GetArea();  //
Sample use of face object pointer

IEntity m\_Entity(faceDisp);
   // Obtain pointer to entity object

faceDisp->AddRef();     //
Manually increment the reference count

boolean retval = m\_Entity.Select(TRUE);
  // Sample use of entity object pointer

faceDisp = m\_Face.GetNextFace();   //
Get the next face

}      //
End while faces exist

      // Objects go out
of scope and ref count decremented in destructor

' In Visual Basic for Applications (VBA)

Dim FaceObj,BodyObj As Object

Dim theFaceArea As Double

Dim ok As Boolean

Set BodyObj = PartObj.Body   '
Get body object from the part

' PartObj represents PartDoc interface - possibly obtained

' using ActiveDoc, OpenDoc, NewPart, etc. functions

If (BodyObj Is Nothing) Then

swApp.SendMsgToUser "Error!
Part has no body."

Exit Sub

End If

Set FaceObj = BodyObj.GetFirstFace  '
Get first face from the body object

While Not FaceObj Is Nothing   '
While faces exist, traverse them

theFaceArea = FaceObj.GetArea  '
Sample use of face object pointer

ok = FaceObj.Select(True)   '
Sample use of entity object pointer

' Face object can be used for entity object calls

Set FaceObj = FaceObj.GetNextFace '
Get the next face

Wend      '
End while faces exist

Set BodyObj = Nothing   '
Clean up variables

Set FaceObj = Nothing

Set PartObj = Nothing

## VARIANT Return Values

SOLIDWORKS might also return an empty or NULL VARIANT. It is also good
programming practice to check for this condition. The following unmanaged
C++ and VBA examples show you one method of checking for an empty VARIANT:

// In unmanaged C++

VARIANT v = m\_ModelDoc.GetMassProperties();  //
Get the mass properties

If ((v.vt == VT\_EMPTY) || (V\_VT(&v)
== VT\_NULL)) // Error occurred

return;

' In Visual Basic for Applications (VBA)

PickPt = m\_SelectionManager.GetSelectionPointInSketchSpace(1)
 ' Get the user's pick point

If (IsEmpty(PickPt) Or IsNull(PickPt))
Then    ' No pick point available

Exit Sub

End If

## SafeArray Return Values

The SOLIDWORKS API passes and returns all SafeArrays as a type VARIANT.
In many instances, you might find it useful to know the length of a SafeArray
returned by SOLIDWORKS. If SOLIDWORKS does not provide a function that
counts, such as IFace2::GetEdgeCount, you can use standard MFC or VBA
routines to determine the SafeArray length. The following unmanaged C++
and VBA examples show you one way for determining the number of elements
in a SafeArray.

// In unmanaged C++

// Get all of the children components from this m\_Component
object

VARIANT componentChildren = m\_Component.GetChildren();

if ((componentChildren.vt == VT\_EMPTY)
||

(V\_VT(&componentChildren)
== VT\_NULL)) // Error - array is empty or null

return;

SafeArray\* psa = V\_ARRAY(&componentChildren);

LPDISPATCH\* componentChildrenArray;

HRESULT hres = SafeArrayAccessData(psa,
(void \*\*)&componentChildrenArray);

long highIndex;

SafeArrayGetUBound(psa, 1, &highIndex); //
Get index number of highest array element

       //
The array range is from 0 to highIndex

long childrenCount = highIndex
+ 1;  // Actual # of array elements is highIndex +
1

for (int i = 0; i < childrenCount;
i++) // For each child component

{

IComponent m\_childComponent(componentChildrenArray[i]);

componentChildrenArray[i]->AddRef();

VARIANT\_BOOL isSuppressed;   //
Perform sample operation using the component

isSuppressed = m\_childComponent.IsSuppressed();

}

hres = SafeArrayUnaccessData(psa);  //
Release and destroy the

hres = SafeArrayDestroy(psa);   //
component SafeArray

' In VBA

' Display the entire version history for the
specified file

' Show results in a list box control

Dim fileHistory As Variant

fileHistory = swApp.VersionHistory(filename)

If Not (IsEmpty(fileHistory) Or
IsNull(fileHistory)) Then

For i = 0 To UBound(history)   ' For each
string in the SafeArray,

myListBox.AddItem (fileHistory(i))  '
Display it in the list box control

Next i

End If