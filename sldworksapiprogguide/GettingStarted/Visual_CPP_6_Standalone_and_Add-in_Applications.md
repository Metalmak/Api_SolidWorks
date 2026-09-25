<!-- source: sldworksapiprogguide/GettingStarted/Visual_CPP_6_Standalone_and_Add-in_Applications.htm -->

# SOLIDWORKS API Help

# Visual C++ 6.0 Standalone and Add-in Applications

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

. // Your
code

.

//Shut down SOLIDWORKS

swApp->ExitApp();

//Release COM reference

swApp = NULL;

//Uninitialize COM

CoUninitialize();

return 0;

}

## Add-in Applications (.dll files)

Visual C++ applications have the option of using a COM or Dispatch interface.
See [COM vs. Dispatch](../Overview/COM_vs_Dispatch.htm) for
details.

NOTE: For COM DLL add-ins, success
or failure on import/export is returned by the add-in through the HRESULT.