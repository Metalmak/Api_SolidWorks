<!-- source: sldworksapiprogguide/Overview/SelectionManagerCPPCLI.htm -->

# SOLIDWORKS API Help

# SelectionManager.cpp Written in C++/CLI

// SelectionManager.cpp : main project file

// Gets the selected objects in the active model document

#include "stdafx.h"

using namespace System;

// Add the SOLIDWORKS Primary interop assemblies to
the references

using namespace SolidWorks::Interop::sldworks;

using namespace SolidWorks::Interop::swconst;

int main(array<System::String ^> ^args)

{

ISldWorks^    swApp;

swApp = gcnew SldWorksClass;

if (! swApp) {

return(0);

}

swApp->UserControl = true;

swApp->Visible = true;

IModelDoc2^  swModel;

swModel = swApp->IActiveDoc2;

if (! swModel) {

return(0);

}

String^            strModelTitle;

swDocumentTypes\_e  nDocumentType;

strModelTitle = swModel->GetTitle();

nDocumentType = (swDocumentTypes\_e)swModel->GetType();

ISelectionMgr^     swSelectionManager;

swSelectType\_e     nSelectionType;

Object^            swSelectedObject;

IFace2^            swFace;

IEdge^             swEdge;

swSelectionManager = swModel->ISelectionManager;

for (int i = 1; i <= swSelectionManager->GetSelectedObjectCount2(-1);
i++) {

swSelectedObject = swSelectionManager->GetSelectedObject6(i,
-1);

nSelectionType = (swSelectType\_e)swSelectionManager->GetSelectedObjectType3(i,
-1);

switch (nSelectionType) {

case swSelectType\_e::swSelFACES:

swFace =  (Face2^)swSelectedObject;

break;

case swSelectType\_e::swSelEDGES:

swEdge = (Edge^)swSelectedObject;

break;

}

}

return(0);

}