<!-- source: sldworksapi/SelectionManagerCPP.htm -->

# SOLIDWORKS API Help

# SelectionManager.cpp Written in C++

// SelectionManager.cpp : Defines the entry point for
the console application

// Gets the selected objects in the active model document

#include "stdafx.h"

// Add the path to the SOLIDWORKS type libraries to
the "Additional Include Directories".

#import "sldworks.tlb" raw\_interfaces\_only,
raw\_native\_types, no\_namespace, named\_guids  //
SOLIDWORKS type library

#import "swconst.tlb" raw\_interfaces\_only,
raw\_native\_types, no\_namespace, named\_guids   //
SOLIDWORKS constants type library

int \_tmain(int argc, \_TCHAR\* argv[])

{

// Initialize COM

// Do this before using ATL smart pointers
so COM is available

CoInitialize(NULL);

// Use a block so the smart pointers are
destructed when the scope of this block is left

{

// Use ATL smart pointers

CComPtr<ISldWorks>   swApp;

if(swApp.CoCreateInstance(\_\_uuidof(SldWorks),
NULL, CLSCTX\_LOCAL\_SERVER) != S\_OK) {

return(0);

}

swApp->put\_UserControl(VARIANT\_TRUE);

swApp->put\_Visible(VARIANT\_TRUE);

CComPtr<IModelDoc2>  swModel;

swApp->get\_IActiveDoc2(&swModel);

if (! swModel) {

return(0);

}

CComBSTR  strModelTitle;

long      nDocumentType;
 // swDocumentTypes\_e

swModel->GetTitle(&strModelTitle);

swModel->GetType(&nDocumentType);

CComPtr<ISelectionMgr>     swSelectionManager;

long                       lNumSelections;

long                       nSelectionType;
    //
swSelectType\_e

CComPtr<IDispatch>         swSelectedObject;

CComPtr<IFace2>            swFace;

CComPtr<IEdge>             swEdge;

swModel->get\_ISelectionManager(&swSelectionManager);

swSelectionManager->GetSelectedObjectCount2(-1,
&lNumSelections);

for (int i = 1; i <= lNumSelections;
i++) {

swSelectionManager->GetSelectedObject6(i,
-1, &swSelectedObject);

swSelectionManager->GetSelectedObjectType3(i,
-1, &nSelectionType);

switch (nSelectionType) {

case swSelectType\_e::swSelFACES:

swSelectedObject.QueryInterface(&swFace);

break;

case swSelectType\_e::swSelEDGES:

swSelectedObject.QueryInterface(&swEdge);

break;

}

}

}

// ATL smart pointers are destructed so
all COM objects you held on to are released

// Now you can safely shut down COM as you
do not need it any longer

// Stop COM

CoUninitialize();

return(0);

}