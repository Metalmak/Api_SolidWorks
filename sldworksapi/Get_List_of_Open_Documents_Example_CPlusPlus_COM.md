<!-- source: sldworksapi/Get_List_of_Open_Documents_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get List of Open Documents Example (C++ COM)

This example shows how to get a list of the currently open SOLIDWORKS
documents.

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

    CComPtr<IEnumDocuments2>
               pEnumDoc;

    long
                                   nFetched
= -1;

    CComPtr<IModelDoc2>
                    pModelDoc;

    long
                                   i
= -1;

    //
Connect to SOLIDWORKS application

    pSldWorks
= TheApplication->GetSWApp();

    ASSERT(pSldWorks);

    hr
= pSldWorks->EnumDocuments2(&pEnumDoc);

    ASSERT(pEnumDoc);

    hr
= pEnumDoc->Reset();

    do

        {

        CComBSTR
                               sPathName;

        //
Reset before reuse

        pModelDoc
= NULL;

        //
Could also check HRESULT or nFetched

        hr
= pEnumDoc->Next(1, &pModelDoc,
&nFetched);

        if
(pModelDoc)

            {

            //
Debugging only

            hr
= pModelDoc->GetPathName(&sPathName);

            }

        }
while (pModelDoc);

    return;

} //void APITestFunction()

// -------------------------------------------------------------------