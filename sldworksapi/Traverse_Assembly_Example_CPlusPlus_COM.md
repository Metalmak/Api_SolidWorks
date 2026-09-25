<!-- source: sldworksapi/Traverse_Assembly_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Traverse Assembly Example (C++ COM)

This example shows how to traverse an assembly
using the IComponent2 object. The method IComponent2::IGetChildren returns
an array, so this code must be used in an in-process DLL. Otherwise, use
the method IComponent2::GetChildren that returns a VARIANT.

void GetModelAssembly(ISldWorks\* m\_pSldWorks)

{

 LPCONFIGURATION
pConfiguration = NULL;

 LPCOMPONENT
pRootComponent = NULL;

 LPMODELDOC2
pModelDoc = NULL;

 HRESULT
hres = S\_OK;

 long
RecurseLevel = 0;

 hres
= m\_pSldWorks->get\_IActiveDoc2(
&pModelDoc );

 //
Retrieve model document pointer

 if(
S\_OK != hres || pModelDoc == NULL )

  return;

 //
Get the active configuration and root component

 if
( pModelDoc->IGetActiveConfiguration(&pConfiguration)
== S\_OK )

 {

  if
( pConfiguration->IGetRootComponent(&pRootComponent)
== S\_OK )

  {

   CString
MyString;

   TraverseChildren(RecurseLevel,&MyString,pRootComponent);

   pRootComponent->Release();

   //
Display the structure in a message box

   AfxMessageBox
(MyString);

  }

  pConfiguration->Release();

 }

 pModelDoc->Release();

}

//////////////////////////////////////////////////////////////////////////

// Function: TraverseChildren

// Arguments: RecurseLevel - Level of recursion

//    MyString
- Textural record of assembly

//    pComponent
- Component to traverse

// Return: Number of children

// Description: Perform any operations specific to the
component, then

//    if
the component has children, recursively call

//    this
function for each child.

//////////////////////////////////////////////////////////////////////////

int TraverseChildren(long RecurseLevel, CString\* MyString,
LPCOMPONENT pComponent)

{

 LPCOMPONENT\*
pChildren = NULL;

 int
  nChildren;

 int
  i;

 BSTR
  Name;

 HRESULT
 hres =
S\_OK;

 LPMODELDOC
 pModelDoc
= NULL;

 //
Retrieve the component name

 if(RecurseLevel==0)

 {

  //
Special case of top-level components

  hres
= m\_pSldWorks->get\_IActiveDoc(
&pModelDoc );

  if(
S\_OK == hres || pModelDoc != NULL )

   hres
= pModelDoc->GetTitle(&Name);

 }

 else

 {

  //
Get the component name

  hres
= pComponent->get\_Name(&Name);

 }

 if(
S\_OK == hres && Name != NULL )

 {

  CString
tempstr;

  for(
i=1; I<=RecurseLevel; i++)

  {

   tempstr
+= " ";

  }

  CString
Tmp(Name);

  tempstr
+= Tmp;

  tempstr
+= "\r\n";

  \*MyString
= \*MyString + tempstr;

 }

 RecurseLevel++;

 hres
= pComponent->IGetChildrenCount(&nChildren);

 //
Check if this component has children

 if
( S\_OK == hres || nChildren > 0 )

 {

  pChildren
= new LPCOMPONENT [nChildren];

  hres
= pComponent->IGetChildren((LPCOMPONENT\*\*)&pChildren);

  if(S\_OK
== hres)

  {

   //
Recursively traverse the children

   for
( i=0; i<nChildren; i++ )

   {

    TraverseChildren(RecurseLevel,MyString,pChildren[i]);

    pChildren[i]->Release();

   }

  }

  delete
[] pChildren;

 }

 RecurseLevel--;

 return
nChildren;

}