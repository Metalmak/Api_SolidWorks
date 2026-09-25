<!-- source: sldworksapi/Get_Bodies_in_Components_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get Bodies in Components Example (C++ COM)

This example shows how to get the bodies in assembly components.

// -------------------------------------------------------------------

void
CSwAddin2::GetBodiesOfComponents()

{

     HRESULT hr = S\_OK;

     VARIANT\_BOOL bRet = VARIANT\_FALSE;

     long
nRetVal = -1;

     CComPtr <IModelDoc2> pModel;

     CComQIPtr <IAssemblyDoc> pAssembly;

     CComQIPtr <IComponent2> pComponent;

     CComQIPtr <IBody2> pBody;

     VARIANT vComponents;

     VARIANT vBodyArr;

     VARIANT vBodyInfo;

     long
Count;

     long
nCopmCount;

     long
CntBody;

     long
BodyCount;

     SAFEARRAY\* psaBody;

     hr = iSwApp->**get\_IActiveDoc2**(&pModel);

     ASSERT(pModel);

     pAssembly = pModel;

     ASSERT(pAssembly);

     hr = pAssembly->**GetComponents**(VARIANT\_TRUE,&vComponents);

     ASSERT(NULL!= vComponents.pparray);

     SAFEARRAY\* psaComp = V\_ARRAY(&vComponents);

     LPDISPATCH\* pCompDispArray = NULL;

     hr = SafeArrayAccessData(psaComp,(void\*\*)&pCompDispArray);

     hr =
SafeArrayGetUBound(psaComp,1,&Count);

     nCopmCount = Count+1;

     for(int
i = 0; i < nCopmCount; i++)

     {

          CComBSTR sCompMateName (L"");

          CComBSTR sBodyName (L"");

          CComQIPtr <IComponent2> pComp;

          pComp = pCompDispArray[i];

          pComp->**get\_Name2**(&sCompMateName);

          pComp->**GetBodies3**(0,&vBodyInfo,&vBodyArr);

          ASSERT(NULL!= vBodyArr.pparray);

          psaBody = V\_ARRAY(&vBodyArr);

          LPDISPATCH\* pBodyDispArray =
NULL;

          hr =
SafeArrayAccessData(psaBody,(void\*\*)&pBodyDispArray);

          hr =
SafeArrayGetUBound(psaBody,1,&CntBody);

          BodyCount = CntBody+1;

          for(int
j = 0; j < BodyCount; j++)

          {

              pBody = pBodyDispArray[j];

              pBody->**get\_Name**(&sBodyName);

          }

          hr =
SafeArrayUnaccessData(psaBody);

          hr = SafeArrayDestroy(psaBody);

     }

     hr = SafeArrayUnaccessData(psaComp);

     hr = SafeArrayDestroy(psaComp);

}