<!-- source: sldworksapi/Get_and_Set_Units_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get and Set Units Example (C++ COM)

This example shows how to get the current unit
settings of the document and change them to inches. Be sure to import
swconst.tlb.

The method IModelDoc2::IGetUnits returns an
array, so this code must be used in an in-process DLL. Otherwise, use
the method IModelDoc2::GetUnits that returns a VARIANT.

GetAndSetUnits(ISldWorks\* m\_pSldWorks)

{

 LPMODELDOC2
pModelDoc = NULL;

 //
Retrieve Model Document pointer

 if(
S\_OK != m\_pSldWorks->get\_IActiveDoc2(
&pModelDoc ) || pModelDoc == NULL )

  return;

 short
unitArray[5];

 HRESULT
hres = S\_OK;

 hres
= pModelDoc->IGetUnits(unitArray);

 CString
message;    //
Create message string

 message.Format(\_T("Unit
Settings are:\n%d \t%d \t%d \t%d \t%d"),

 unitArray[0],unitArray[1],unitArray[2],unitArray[3],unitArray[4]);

 //
Send message to the user

 AfxMessageBox
(message);

 //
If units are not inches, change them to inches

 if
(unitArray[0] != swINCHES)

 {

  short
denom = 16;

  hres
= pModelDoc->SetUnits(swINCHES,
swFRACTION, denom, unitArray[3], FALSE);

 }

 pModelDoc->Release();

}