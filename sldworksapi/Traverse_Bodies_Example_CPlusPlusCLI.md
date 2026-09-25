<!-- source: sldworksapi/Traverse_Bodies_Example_CPlusPlusCLI.htm -->

# SOLIDWORKS API Help

# Traverse Bodies (C++/CLI)

This example shows how to traverse bodies.

//----------------------------------------------------------------------------

// BodyTraversal.cpp : main project file.

//

// Preconditions: Model document is open.

//

// Postconditions: None

//----------------------------------------------------------------------------

#include "stdafx.h"

using namespace System;

// Add the SOLIDWORKS primary interop assemblies to
the references

using namespace SOLIDWORKS::Interop::sldworks;

using namespace SOLIDWORKS::Interop::swconst;

int main(array<System::String ^> ^args)

{

ISldWorks^    swApp;

swApp = gcnew SldWorksClass;

if (! swApp) {

return(0);

}

swApp->UserControl
= true;

swApp->Visible
= true;

IModelDoc2^  swModel;

swModel = swApp->IActiveDoc2;

if (! swModel) {

return(0);

}

IModelDocExtension^     swModelExtension;

swModelExtension = swModel->Extension;

String^            strModelTitle;

swDocumentTypes\_e  nDocumentType;

strModelTitle = swModel->GetTitle();

nDocumentType = (swDocumentTypes\_e)swModel->GetType();

if (nDocumentType != swDocumentTypes\_e::swDocPART)
{

return(0);

}

IPartDoc^   swPart
= nullptr;

swPart = (IPartDoc^)swModel;

array<Object^>^  aBodies;

aBodies = safe\_cast<array<Object^>^>(swPart->GetBodies2((int)swBodyType\_e::swSolidBody,
true));

swModel->ClearSelection2(true);

for each (IBody2^ swBody in aBodies) {

System::Console::WriteLine("Old name
= " + swBody->Name);

swBody->Name
= swBody->Name + "\_renamed";

bool bSelected = swModelExtension->SelectByID2(swBody->Name, "SOLIDBODY",
0.0, 0.0, 0.0, true, 0, nullptr, (int)swSelectOption\_e::swSelectOptionDefault);

System::Console::WriteLine("New name
= " + swBody->Name);

IFace2^   swFace
= nullptr;

//swFace = (IFace2^)swBody->GetFirstFace();

swFace = swBody->IGetFirstFace();

while (swFace != nullptr) {

int iNumEdges = swFace->GetEdgeCount();

//swFace = (IFace2^)swFace->GetNextFace();

swFace = swFace->IGetNextFace();

}

}

bool bStatus = swModel->EditRebuild3();

return(0);

}