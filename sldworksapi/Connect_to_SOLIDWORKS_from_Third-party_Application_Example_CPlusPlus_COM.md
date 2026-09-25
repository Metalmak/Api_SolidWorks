<!-- source: sldworksapi/Connect_to_SOLIDWORKS_from_Third-party_Application_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Connect to SOLIDWORKS from Third-party Application Example (C++)

This example shows how to connect to SOLIDWORKS from a third-party application
using C++.

// HelloSW.cpp : Defines the entry point for the console
application.

//

#include "stdafx.h"

#include "objbase.h"

#import "sldworks.tlb" no\_namespace raw\_interfaces\_only

int \_tmain(int argc, \_TCHAR\* argv[])

{

::CoInitialize(NULL);

{

CLSID clsid;

::CLSIDFromProgID(L"SldWorks.Application",
&clsid);

ISldWorks \*swApp = NULL;

::CoCreateInstance(clsid, NULL, CLSCTX\_LOCAL\_SERVER,
\_\_uuidof(ISldWorks), (void\*\*)&swApp);

if (swApp != NULL)

{

BSTR bstrHello = ::SysAllocString(L"Hello
from SOLIDWORKS.");

swApp->SendMsgToUser(bstrHello);

::SysFreeString(bstrHello);

swApp->Release();

}

}

::CoUninitialize();

return 0;

}