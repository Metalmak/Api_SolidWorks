<!-- source: sldworksapi/QueryInterface_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Use QueryInterface Example (C++ COM)

This example shows how to use QueryInterface.

LPUNKNOWN iUnk = NULL;

LPFEATURE m\_Feature = NULL;

HRESULT hres = S\_FALSE;

// Your code

...

// Get the underlying object

hres = m\_Feature->IGetSpecificFeature(
&iUnk );

LPREFPLANE m\_RefPlane = NULL;

hres = iUnk->QueryInterface(
IID\_IRefPlane, (LPVOID\*)&m\_RefPlane);

// If Feature is a RefPlane

if (hres == S\_OK && m\_RefPlane
!= NULL)

{

AfxMessageBox( \_T("This feature is a reference plane") );

// Use m\_RefPlane object

...

// Release m\_RefPlane object

m\_RefPlane->Release();

}

// Release iUnk object

iUnk->Release();

/\*

   The
call to IGetSpecificFeature increases the reference count on iUnk by 1.
If the call to QueryInterface is successful, it also increases the reference
count on iUnk by 1. The m\_RefPlane and iUnk pointers are the same object;
you can therefore release either one. m\_RefPlane->Release()
is shown in this example.

\*/