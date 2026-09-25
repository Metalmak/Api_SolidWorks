<!-- source: sldworksapi/Open_Assembly_Component_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Open Assembly Component Example (C++ COM)

This example shows how to open a component that is part of the current
assembly document.

// Your code

...

LPMODELDOC m\_ModelDoc = NULL;

 HRESULT hres = NOERROR;

 //
Retrieve IModelDoc pointer

 hres = UserApp->getSWApp()->get\_IActiveDoc( &m\_ModelDoc );

 if( m\_ModelDoc == NULL
)

  return;

 LPASSEMBLYDOC m\_AssemblyDoc
= NULL;

 hres = m\_ModelDoc->QueryInterface(IID\_IAssemblyDoc,
(LPVOID \*)&m\_AssemblyDoc);

 // If current document
is not an assembly then return

 if(hres!=S\_OK || m\_AssemblyDoc==NULL)

return;

 VARIANT\_BOOL selOK;

 hres = m\_ModelDoc->SelectByID(\_T("Lever-1@LeverAssem"),
\_T("COMPONENT"), 0, 0, 0, &selOK);

 // Open the component
file

 hres = m\_AssemblyDoc->OpenCompFile();

 //
Make the Lever component the active document

 //
Note: Use the correct filename extension

 hres = m\_pSOLIDWORKS->IActivateDoc(\_T("Lever.SLDPRT"),
&m\_ModelDoc);

// Your code

...

 // Releasing

 m\_AssemblyDoc->Release();

 m\_ModelDoc->Release();