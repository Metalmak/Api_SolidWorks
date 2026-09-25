<!-- source: sldworksapi/Traverse_All_Open_Documents_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Traverse All Open Documents Example (C++ COM)

This example shows how to traverse all open
documents.

bool CFileReferenceTests::isFileOpen(CString
fileSpec)

{

 bool retval = FALSE;

 HRESULT hres = S\_FALSE;

 if (fileSpec.IsEmpty())

  return retval;

 LPENUMDOCUMENTS pDocEnum
= NULL;

 hres = TheApplication->m\_pSldWorks->EnumDocuments2(&pDocEnum);

 // No documents
open

 if (pDocEnum == NULL)

  return retval;

 int docNum = 0;

 LPMODELDOC pModelDoc =
NULL;

 hres = pDocEnum->Next(1,
&pModelDoc, NULL);

 while (S\_OK == hres)

 {

  BSTR bdocName;

  hres = pModelDoc->GetPathName(&bdocName);

  CString docName(bdocName);

  //
File name matches

  if (fileSpec.CompareNoCase(docName)
== 0)

   retval = TRUE;

  pModelDoc->Release();

  pModelDoc = NULL;

  hres = pDocEnum->Next(1, &pModelDoc, NULL);

 }

 if (pDocEnum != NULL)
pDocEnum->Release();

 return retval;

}