<!-- source: sldworksapi/Set_View_Display_Mode_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Set View Display Mode Example (C++ COM)

This example shows how to set the display mode of drawing views.

STDMETHODIMP CDgtlPen::demo2()

{

    HRESULT
                                hr
= S\_OK;

    CComPtr
<IModelDoc2>                    pModel;

    CComQIPtr
<IDrawingDoc>                 pDraw;

    CComPtr
<ISheet>                        pSheet;

    CComPtr
<IView>                         pSheetView;

    CComPtr
<IView>                         pView;

    long
                                   swDisplayMode
= -1;

    VARIANT\_BOOL
                           UseParent
= FALSE;

    VARIANT\_BOOL
                           Facetted
= TRUE;

    VARIANT\_BOOL
                           Edges
= TRUE;

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

    hr
= pDraw->IGetFirstView(&pSheetView);

    \_ASSERT(pSheetView);

    hr
= pSheetView->IGetNextView(&pView);

    \_ASSERT(pView);

    while(pView
!= NULL)

    {

        CComPtr
<IView>                     pNextView;

        hr
= pView->GetDisplayMode2(&swDisplayMode);

        switch(swDisplayMode)

        {

            case
swWIREFRAME:

            case
swHIDDEN\_GREYED:

            case
swHIDDEN:

                break;

            case
swSHADED:

            case
swFACETED\_WIREFRAME:

            case
swFACETED\_HIDDEN\_GREYED:

            case
swFACETED\_HIDDEN:

                hr
= pView->SetDisplayMode3(UseParent,
swHIDDEN, Facetted, Edges, &retval);

                \_ASSERT(retval);

                break;

            default
:

                \_ASSERT(FALSE);

                break;

        }

        hr
= pView->IGetNextView(&pNextView);

        //
Release view

        pView
= NULL;

        pView
= pNextView;

    }

    return
S\_OK;

}