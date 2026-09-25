<!-- source: sldworksapi/Get_Bodies_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get Bodies Example (C++ COM)

This example shows how to get the bodies in a part document.

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

    CComQIPtr
<IPartDoc>                    pPart;

    VARIANT
                            vBodyArr;

    long
                                   i
= -1;

    //
Connect to SOLIDWORKS

    pSldWorks
= TheApplication->GetSWApp();

    ASSERT(pSldWorks);

    hr
= pSldWorks->get\_IActiveDoc2(&pModel);

    ASSERT(pModel);

    hr
= pModel->ClearSelection2(VARIANT\_TRUE);

    pPart
= pModel;

    ASSERT(pPart);

    hr
= pPart->GetBodies2(swSolidBody,
VARIANT\_TRUE, &vBodyArr);

    ASSERT(NULL
!= vBodyArr.pparray);

    //
Process bodies

    SAFEARRAY\*
             psaBody
= V\_ARRAY(&vBodyArr);

    LPDISPATCH\*
            pBodyDispArray
= NULL;

    long
                   nBodyHighIndex
= -1;

    long
                   nBodyCount
= -1;

    hr
= SafeArrayAccessData(psaBody, (void \*\*) &pBodyDispArray);

    ASSERT(S\_OK
== hr);

    ASSERT(NULL
!= pBodyDispArray);

    //
Get index number of highest array element

    //
The array range is from 0 to highIndex

    hr
= SafeArrayGetUBound(psaBody, 1, &nBodyHighIndex);

    ASSERT(S\_OK
== hr);

    //
Actual number of array elements is nBodyHighIndex + 1

    nBodyCount
= nBodyHighIndex + 1;

    //
Process each body

    for
(i = 0; i < nBodyCount; i++)

        {

        CComQIPtr
<IBody2>          pBody;

        //
Calls AddRef() on IDispatch ---> refcount = 2

        pBody
= pBodyDispArray[i];

        ASSERT(pBody);

        hr
= pBody->Select(VARIANT\_TRUE,
0, &bRet);

        ASSERT(bRet);

        //
After this call ---> refcount = 1

        //
When it goes out of scope ---> refcount = 0

        pBody.Release();

        }

    //
Unaccess & destroy the component SafeArray

    hr
= SafeArrayUnaccessData(psaBody);

    hr
= SafeArrayDestroy(psaBody);

    return;

} //void APITestFunction()

// -------------------------------------------------------------------