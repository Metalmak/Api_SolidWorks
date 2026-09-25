<!-- source: sldworksapi/Get_Configuration_Parameters_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get Configuration Parameters Example (C++ COM)

This example shows how to get the parameters for the specified configuration.

'--------------------------------

'

' Preconditions: Part is open and has a configuration
named aaa.

'

' Postconditions: None

'

'---------------------------------

#define USING\_DEBUG\_SOLIDWORKS          TRUE

#ifdef \_DEBUG && USING\_DEBUG\_SOLIDWORKS

    #define
AFX\_MANAGE\_STATE\_ADDIN      AFX\_MANAGE\_STATE(AfxGetAppModuleState());

#else

    #define
AFX\_MANAGE\_STATE\_ADDIN      AFX\_MANAGE\_STATE(AfxGetStaticModuleState());

#endif

// -------------------------------------------------------------------

STDMETHODIMP CAPITestATL::API\_Test(void)

{

    AFX\_MANAGE\_STATE\_ADDIN;

    HRESULT
                            hr
= S\_OK;

    CComPtr
<ISldWorks>                 pSldWorks;

    CComPtr
<IModelDoc2>                pModel;

    CComPtr
<IConfigurationManager>     pCfgMgr;

    CComBSTR
                           sCfgName(\_T("aaa"));

    long
                               NumParams
= 0;

    long
                               i
= 0;

BSTR                                \*vNames
= NULL;

BSTR                                \*vValues
= NULL;

VARIANT\_BOOL                        bret
= VARIANT\_FALSE;

    try

        {

        //
Connect to SOLIDWORKS

        ASSERT(m\_iSldWorks);

        hr
= m\_iSldWorks->get\_IActiveDoc2(&pModel);

        ASSERT(pModel);

        hr
= pModel->get\_ConfigurationManager(&pCfgMgr);

        ASSERT(pCfgMgr);

        hr
= pCfgMgr->GetConfigurationParamsCount(sCfgName,
&NumParams);

        ASSERT(NumParams
> 0);

        vNames
 = new BSTR[NumParams];
 ASSERT(vNames
);

        vValues
= new BSTR[NumParams];  ASSERT(vValues);

        hr
= pCfgMgr->IGetConfigurationParams(sCfgName,
NumParams, vNames, vValues, &bret);

        ASSERT(bret);

        for
(i = 0; i < NumParams; i++)

            {

            CComBSTR
               sName
;

            CComBSTR
               sValue;

            sName
.Attach(vNames [i]);

            sValue.Attach(vValues[i]);

            OutputDebugString(sName
);

            OutputDebugString(\_T("\n"));

            OutputDebugString(sValue);

            OutputDebugString(\_T("\n"));

            }

        delete
[] vNames ;

        delete
[] vValues ;

        }

    catch
(...)

        {

        DebugBreak();

        }

    delete
[] vNames ;

    delete
[] vValues ;

return S\_OK;

}