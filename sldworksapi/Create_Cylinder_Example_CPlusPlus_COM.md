<!-- source: sldworksapi/Create_Cylinder_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Create Cylinder Example (C++ COM)

This example shows how to create a cylinder.

'------------------------------------

'

' Preconditions: None.

'

' Postconditions: A cylinder is created.

'

'------------------------------------

#include "stdafx.h"

#include "CreateCylinder.h"

#ifdef \_DEBUG

#define new DEBUG\_NEW

#undef THIS\_FILE

static char THIS\_FILE[] = \_\_FILE\_\_;

#endif

#include <atlbase.h>

#import "sldworks.tlb" no\_namespace raw\_interfaces\_only

#import "swconst.tlb" no\_namespace

/////////////////////////////////////////////////////////////////////////////

// The one and only application object

CWinApp theApp;

using namespace std;

int \_tmain(int argc, TCHAR\* argv[], TCHAR\* envp[])

{

int nRetCode = 0;

// initialize MFC and print and error on
failure

if (!AfxWinInit(::GetModuleHandle(NULL),
NULL, ::GetCommandLine(), 0))

{

// TODO: change error code to suit your
needs

cerr << \_T("Fatal Error: MFC
initialization failed") << endl;

nRetCode = 1;

}

else

{

::CoInitialize(NULL);

{

VARIANT\_BOOL bRetval = VARIANT\_FALSE;

CComPtr<ISldWorks> swApp;

swApp.CoCreateInstance(L"SldWorks.Application",
NULL, CLSCTX\_LOCAL\_SERVER);

CComPtr<IModelDoc2> swDoc;

CComPtr<IModelDocExtension> swDocExt;

CComPtr<IFeatureManager> swFeatMgr;

swApp->get\_IActiveDoc2(&swDoc);

swDoc->get\_Extension(&swDocExt);

swDoc->get\_FeatureManager(&swFeatMgr);

CComPtr<ISketch> swSketch;

swDoc->IGetActiveSketch2(&swSketch);

if (swSketch == NULL)

{

swDocExt->SelectByID2(L"Front
Plane", L"PLANE", 0.0, 0.0, 0.0, VARIANT\_FALSE, 0, NULL,
swSelectOptionDefault, &bRetval);

swDoc->InsertSketch2(VARIANT\_TRUE);

}

CComPtr<ISketchSegment> swSkSeg;

swDoc->ICreateCircle2(0.0,
0.0, 0.0, 0.025, 0.0, 0.0, &swSkSeg);

CComPtr<IFeature> swFeat;

swFeatMgr->FeatureExtrusion2(VARIANT\_FALSE,
VARIANT\_FALSE, VARIANT\_FALSE,

0, 0, 0.100, 0.100,

VARIANT\_FALSE, VARIANT\_FALSE, VARIANT\_FALSE,
VARIANT\_FALSE, 0.0, 0.0,

VARIANT\_FALSE, VARIANT\_FALSE, VARIANT\_FALSE,
VARIANT\_FALSE,

VARIANT\_TRUE, VARIANT\_FALSE, VARIANT\_TRUE,
0, 0.0, VARIANT\_FALSE, &swFeat);

}

::CoUninitialize();

}

return nRetCode;

}