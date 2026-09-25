<!-- source: sldworksapi/Add_Component_and_Mate_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Add Component and Mate Example (C++ COM)

This example shows how to add a component and mate to an assembly.

* [AddMate.cpp](#AddMate)
* [stdafx.h](#stdafx)
* [stdafx.cpp](#stdcpp)

### AddMate.cpp

////////////////////////////////////////////////////////////

//

// Preconditions: The specified assembly (lens\_mount.sldasm)
and component

//                (camtest.sldprt) files exist.

//

// NOTE: The assembly
and component files are installed when you

//       install
SOLIDWORKS and are intended for the SOLIDWORKS Toolbox

//       tutorial,
so do not save the assembly after running the program.

//

// Postconditions: The component and a mate, called top\_coinc\_camtest-1,

//       are
added to the assembly.

//

///////////////////////////////////////////////////////////

#include "stdafx.h"

using namespace std;

int \_tmain(int argc, \_TCHAR\* argv[])

{

//Initialize COM

CoInitialize(NULL);

//Use ATL smart pointers

CComPtr<ISldWorks> swApp;

CComPtr<IModelDoc2> swModel;

CComPtr<IModelDocExtension> swDocExt;

CComPtr<IAssemblyDoc> swAssy;

CComPtr<IComponent2> swComponent;

CComPtr<IFeature> mateFeature;

CComPtr<IModelDoc2> tmpObj;

CComPtr<IMate2> swMate;

long lErrors;

long lWarnings;

long lMateError;

HRESULT hres = NOERROR;

VARIANT\_BOOL retVal = VARIANT\_FALSE;

//Connect to currently running instance
of SOLIDWORKS

hres = swApp.CoCreateInstance(\_\_uuidof(SldWorks),
NULL, CLSCTX\_LOCAL\_SERVER);

//Open the assembly document

CComBSTR sAssemblyName(L"C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2018\\samples\\tutorial\\toolbox\\lens\_mount.sldasm");

CComBSTR sDefaultConfiguration(L"Default");

swApp->OpenDoc6(sAssemblyName,
swDocASSEMBLY, swOpenDocOptions\_Silent, sDefaultConfiguration, &lErrors,
&lWarnings, &swModel);

swModel = NULL;

//Open the component (part) document

CComBSTR sCompName(L"C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2018\\samples\\tutorial\\toolbox\\camtest.sldprt");

swApp->OpenDoc6(sCompName,
swDocPART, swOpenDocOptions\_Silent, sDefaultConfiguration, &lErrors,
&lWarnings, &tmpObj);

//Re-activate the assembly document

swApp->IActivateDoc3(sAssemblyName,
true, &lErrors, &swModel);

swAssy = swModel;

//Add the component to the assembly

swAssy->AddComponent4(sCompName,
sDefaultConfiguration, -1, -1, -1, &swComponent);

//Concatenate strings for name of mate

CComBSTR sMateName(L"top\_coinc\_");

CComBSTR sCompMateName (L"");

swComponent->get\_Name2(&sCompMateName);

sMateName.AppendBSTR(sCompMateName);

CComBSTR sFullCompMateName = sMateName;

//Concatenate strings for name of first
selection: Top plane of component

CComBSTR sFirstSelection(L"Top@");

sFirstSelection.AppendBSTR(sCompMateName);

CComBSTR sAtSign(L"@");

sFirstSelection.AppendBSTR(sAtSign);

CComBSTR sAssemblyFilename(L"lens\_mount");

sFirstSelection.AppendBSTR(sAssemblyFilename);

//Second selection: Front plane of assembly

CComBSTR sSecondSelection(L"Front@");

//Adjust the view so that you can see the
assembly and the added component

CComBSTR sNamedView(L"\*Trimetric");

swModel->ShowNamedView2(sNamedView,
-1);

swModel->ViewZoomtofit2();

swModel->ClearSelection2(true);

swModel->get\_Extension(&swDocExt);

//Select the planes to mate

CComBSTR sPlane(L"PLANE");

swDocExt->SelectByID2(sFirstSelection,
sPlane, 0, 0, 0, true, 1, NULL, swSelectOptionDefault, &retVal);

swDocExt->SelectByID2(sSecondSelection,
sPlane, 0, 0, 0, true, 1, NULL, swSelectOptionDefault, &retVal);

//Mate the selected entitities

swAssy->AddMate3(swMateCOINCIDENT,
swMateAlignALIGNED, false, 0, 0, 0, 0, 0, 0, 0, 0, false, &lMateError,
&swMate);

//Set the name of the mate feature

mateFeature = swMate;

mateFeature->put\_Name(sFullCompMateName);

return 0;

}

[Back to top](#Top)

### stdafx.h

/// stdafx.h : include file for standard system include
files,

// or project-specific include files that are used frequently,
but

// are changed infrequently

//

#pragma once

#define WIN32\_LEAN\_AND\_MEAN // Exclude rarely-used stuff
from Windows headers

#include <stdio.h>

#include <tchar.h>

#define \_ATL\_CSTRING\_EXPLICIT\_CONSTRUCTORS // some CString
constructors will be explicit

#include <windows.h>

#include <atlbase.h>

#include <iostream>

using namespace std;  //Use
the standard C++ libraries for text output.

#import "sldworks.tlb" raw\_interfaces\_only,
raw\_native\_types, no\_namespace, named\_guids  //the
SOLIDWORKS type library

#import "swconst.tlb"  raw\_interfaces\_only,
raw\_native\_types, no\_namespace, named\_guids  //the
SOLIDWORKS constant type library

// TODO: reference additional headers your program requires
here

[Back to top](#Top)

### stdafx.cpp

// stdafx.cpp : source file that includes just the standard
includes

// AddMates.pch will be the pre-compiled header

// stdafx.obj will contain the pre-compiled type information

#include "stdafx.h"

// TODO: reference any additional headers you need in
STDAFX.H

// and not in this file

[Back to top](#Top)