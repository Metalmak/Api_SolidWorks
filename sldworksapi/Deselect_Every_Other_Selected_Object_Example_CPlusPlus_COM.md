<!-- source: sldworksapi/Deselect_Every_Other_Selected_Object_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Deselect Every Other Selected Object Example (C++ COM)

This example shows how to deselect every other object.

// -------------------------------------------------------------------

void APITestFunction()

{

    HRESULT
                                hr
= S\_OK;

    long
                                   bRet
= FALSE;

    long
                                   nRetVal
= -1;

    CComPtr
<ISldWorks>                     pSldWorks;

    CComPtr
<IModelDoc2>                    pModel;

    CComPtr
<ISelectionMgr>                 pSelMgr;

    long\*
                                  nDeSelectArr
= NULL;

    long
                                   nDeSelectCount
= -1;

    long
                                   nOldSelCount
= -1;

    long
                                   nNewSelCount
= -1;

    long
                                   i
= -1;

    //
Connect to SOLIDWORKS application

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
= pSelMgr->GetSelectedObjectCount(&nOldSelCount);

    ASSERT(nOldSelCount
> 1);

    nDeSelectCount
= floor(nOldSelCount / 2);

    nDeSelectArr
= new long[nDeSelectCount];

    ASSERT(nDeSelectArr);

    ZeroMemory(nDeSelectArr,
nDeSelectCount \* sizeof(long));

    for
(i = 0; i < nDeSelectCount; i++)

        {

        //
Deselect every other item

        //
Memory array is 0-based, but SelectionMgr array is 1-based

        nDeSelectArr[i]
= 2 \* i + 1;

        }

    hr
= pSelMgr->IDeSelect(nDeSelectCount,
nDeSelectArr, &bRet);

    ASSERT(bRet);

    hr
= pSelMgr->GetSelectedObjectCount(&nNewSelCount);

    ASSERT(nNewSelCount
== nOldSelCount - nDeSelectCount);

    delete
[] nDeSelectArr;

}

// -------------------------------------------------------------------