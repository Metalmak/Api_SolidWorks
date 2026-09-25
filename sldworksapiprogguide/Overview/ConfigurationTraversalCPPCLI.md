<!-- source: sldworksapiprogguide/Overview/ConfigurationTraversalCPPCLI.htm -->

# SOLIDWORKS API Help

# Get Names of Configurations Example (C++/CLI)

// ConfigurationTraversal.cpp : main project file

// Get names of configurations in the active model document

#include "stdafx.h"

using namespace System;

// Add the SOLIDWORKS primary interop assemblies to
the references

using namespace SOLIDWORKS::Interop::sldworks;

using namespace SOLIDWORKS::Interop::swconst;

int main(array<System::String ^> ^args)

{

SldWorks^    swApp;

swApp = gcnew SldWorksClass;

if (! swApp) {

return(0);

}

IModelDoc2^  swModel;

swModel = swApp->IActiveDoc2;

if (! swModel) {

return(0);

}

String^            strModelTitle;

swDocumentTypes\_e  nDocumentType;

strModelTitle = swModel->GetTitle();

nDocumentType = (swDocumentTypes\_e)swModel->GetType();

array<String^>^ aConfigurationNames;

aConfigurationNames = safe\_cast<array<String^>^>(swModel->GetConfigurationNames());

for each (String^ strConfigurationName in
aConfigurationNames) {

System::Console::WriteLine(strConfigurationName);

}

return(0);

}