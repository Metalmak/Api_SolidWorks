<!-- source: sldworksapi/Get_Sheet_Properties_and_Insert_Object_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get Sheet Properties and Insert Object Example (C++ COM)

This example shows how to get a sheet's properties and then insert an
object from a file.

STDMETHODIMP CDgtlPen::demo1()

{

    HRESULT
                                hr
= S\_OK;

    CComPtr
<IModelDoc2>                    pModel;

    CComQIPtr
<IDrawingDoc>                 pDraw;

    double
                                 pSheetProps[7];

    CComPtr
<ISheet>                        pSheet;

    BOOL
                                   createLink
= FALSE;

    double
                                 x
= 0;

    double
                                 y
= 0;

    double
                                 z
= 0;

    VARIANT\_BOOL
                           retval
= NULL;

    hr
= m\_iSldWorks->get\_IActiveDoc2(&pModel);

    \_ASSERT(pModel);

    pDraw
= pModel;

    \_ASSERT(pDraw);

    hr
= pDraw->IGetCurrentSheet(&pSheet);

    \_ASSERT(pSheet);

    ZeroMemory(pSheetProps,
7 \* sizeof(double));

    hr
= pSheet->IGetProperties(pSheetProps);

    y
= pSheetProps[6];

    hr
= pModel->InsertObjectFromFile
(CComBSTR(\_T("C:/Bitmaps/digitalpen.bmp")), createLink, x, y,
z, &retval);

    return
S\_OK;

}