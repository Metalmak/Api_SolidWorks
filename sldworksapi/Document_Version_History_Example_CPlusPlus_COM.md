<!-- source: sldworksapi/Document_Version_History_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Obtain Version History Example (C++ COM)

This example shows how to obtain a version
history of a file. IModelDoc2::IVersionHistory returns an array, so this
code must be used in an in-process DLL.

DocumentVersionHistory(ISldWorks\* m\_pSldWorks)

{

 BSTR\*
versionHistStrings = NULL;

 LPMODELDOC2
pModelDoc = NULL;

 HRESULT
hres= S\_OK;

 hres
= m\_pSldWorks->get\_IActiveDoc2(&pModelDoc);

 if
(hres != S\_OK || pModelDoc == NULL)

  return;

 int
versHistCount = 0;

 hres
= pModelDoc->IGetVersionHistoryCount(&versHistCount);

 if
(hres != S\_OK || versHistCount == 0)

 {

  pModelDoc->Release();

  return;

 }

 versionHistStrings
= new BSTR[versHistCount];

 hres
= pModelDoc->IVersionHistory(versionHistStrings);

 if
(hres != S\_OK || versionHistStrings == NULL)

 {

  delete
[] versionHistStrings;

  pModelDoc->Release();

  return;

 }

 //
For each version found

 for
(int ii = 0;ii < versHistCount;ii++)

 {

  CString
tempstr2(versionHistStrings[ii]);

  AfxMessageBox
(tempstr2);

  SysFreeString(
versionHistStrings[ii]);

 }

 //
default destructor

 pModelDoc->Release();

 delete
[] versionHistStrings;

}