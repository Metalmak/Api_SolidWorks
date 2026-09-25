<!-- source: sldworksapi/Get_Sketch_Segment_Constraints_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get Sketch Segment Constraints Example (C++ COM)

This example shows how to get the constraints for the selected sketch
segment.

// -------------------------------------------------------------------

void APITestFunction()

{

    HRESULT
                                hr
= S\_OK;

    VARIANT\_BOOL
                           bRet
= VARIANT\_FALSE;

    long
                                   nRetVal
= -1;

    CComPtr
<ISldWorks>                     pSldWorks;

    CComPtr
<IModelDoc2>                    pModel;

    CComPtr
<ISelectionMgr>                 pSelMgr;

    CComPtr
<IUnknown>                      pUnk;

    CComQIPtr
<ISketchSegment>              pSkSeg;

    long
                                   nNumConstr
= -1;

    BSTR\*
                                  pConstrArr
= NULL;

    long
                                   i
= -1;

    //
connect to SW

    pSldWorks
= TheApplication->GetSWApp();

    ASSERT(pSldWorks);

    hr
= pSldWorks->get\_IActiveDoc2(&pModel);

    ASSERT(pModel);

    hr
= pModel->get\_ISelectionManager(&pSelMgr);

    ASSERT(pSelMgr);

    hr
= pSelMgr->IGetSelectedObject5(1,
&pUnk);

    ASSERT(pUnk);

    pSkSeg
= pUnk;

    ASSERT(pSkSeg);

    hr
= pSkSeg->IGetConstraintsCount(&nNumConstr);

    ASSERT
(nNumConstr > 0);

    pConstrArr
= new BSTR[nNumConstr];

    ASSERT(pConstrArr);

    ZeroMemory(pConstrArr,
nNumConstr \* sizeof(BSTR));

    hr
= pSkSeg->IGetConstraints(pConstrArr);

    ASSERT(pConstrArr[0]);

    for
(i = 0; i < nNumConstr; i++)

        {

        CComBSTR
                               sConstrStr;

        sConstrStr.Attach(pConstrArr[i]);

        OutputDebugString(sConstrStr);

        OutputDebugString(\_T("\n"));

        }

    delete
[] pConstrArr;

    return;

} //void APITestFunction()

// -------------------------------------------------------------------