<!-- source: sldworksapiprogguide/GettingStarted/CPP_.NET_Standalone_and_Add-in_Applications.htm -->

# SOLIDWORKS API Help

# Visual C++/CLI Standalone and Add-in Applications

## Standalone Applications (.exe files)

To create an instance of the SOLIDWORKS software, your executable project
should contain lines of code similar to the following:

//Import the SOLIDWORKS type library

#import "[sldworks.tlb](../Overview/Type_Libraries.htm)"
raw\_interfaces\_only, raw\_native\_types, no\_namespace, named\_guids

//Import the SOLIDWORKS constant type library

#import "[swconst.tlb](../Overview/Type_Libraries.htm)"
 raw\_interfaces\_only,
raw\_native\_types, no\_namespace, named\_guids

int \_tmain(int argc, \_TCHAR\* argv[])

{

//Initialize COM

CoInitialize(NULL);

//Use [ATL smart pointers](../Overview/Smart_Pointers.htm)

CComPtr<ISldWorks> swApp;

//Create an instance of SOLIDWORKS

HRESULT hres = swApp.CoCreateInstance(\_\_uuidof(SldWorks),
NULL, CLSCTX\_LOCAL\_SERVER);

.

.             //Your
code

.

//Shut down SOLIDWORKS

swApp->ExitApp();

// Release COM reference

swApp = NULL;

//Uninitialize COM

CoUninitialize();

return 0;

}

## Add-in Applications (.dll files)

You can create a Visual C++/CLI DLL add-in using the
SOLIDWORKS
COM Add-In Wizard included in the [SOLIDWORKS
API SDK](SolidWorks_API_Getting_Started_Overview.htm). See [SOLIDWORKS
COM Addin Wizard](../Overview/Using_SolidWorks_CPlusPlus_NET_Add-In_Wizard_to_Create.htm) for details.