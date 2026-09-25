<!-- source: sldworksapi/Insert_Macro_Feature_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Insert Macro Feature Example (C++ COM)

This example shows how to insert a macro feature.

//-------------------------------------------

void APITestFunction()

{

    HRESULT
                            hr
= S\_OK;

    CComPtr
<ISldWorks>                 pSldWorks;

    CComPtr
<IModelDoc2>                pModel;

    CComQIPtr
<IPartDoc>                pPart;

    CComPtr
<IBody2>                    pBody;

    CComPtr
<IFeatureManager>           pFeatMgr;

    CComPtr
<IFeature>                  pFeat;

    BSTR
                               sMacroMethods[9];

    long
                               i
= -1;

    VARIANT\_BOOL
                       bRet
= VARIANT\_FALSE;

    //
Connect to SOLIDWORKS

    pSldWorks
= TheApplication->GetSWApp();

    ASSERT(pSldWorks);

    hr
= pSldWorks->get\_IActiveDoc2(&pModel);

    ASSERT(pModel);

    pPart
= pModel;

    ASSERT(pPart);

    hr
= pPart->IBodyObject2(&pBody);

    ASSERT(pBody);

    hr
= pModel->get\_FeatureManager(&pFeatMgr);

    ASSERT(pFeatMgr);

    sMacroMethods[0]
= \_T("");

    sMacroMethods[1]
= \_T("");

    sMacroMethods[2]
= \_T("");

    sMacroMethods[3]
= \_T("");

    sMacroMethods[4]
= \_T("");

    sMacroMethods[5]
= \_T("");

    sMacroMethods[6]
= \_T("");

    sMacroMethods[7]
= \_T("");

    sMacroMethods[8]
= \_T("");

    hr
= pFeatMgr->IInsertMacroFeature(

                        CComBSTR(\_T("CeTestMacro")),

                        CComBSTR(\_T("Sample.SimpleExtrude")),

                        sMacroMethods,

                        0,

                        NULL,

                        NULL,

                        NULL,

                        pBody,

                        swMacroFeatureSecurityByDefault,

                        &pFeat);

    ASSERT(pFeat);

} //void APITestFunction()

// -------------------------------------------------------------------