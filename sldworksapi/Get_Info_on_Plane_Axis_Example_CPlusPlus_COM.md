<!-- source: sldworksapi/Get_Info_on_Plane_Axis_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get Info on Plane/Axis Example (C++ COM)

This example shows how to get parameter information
for the currently selected reference plane or reference axis.

void GetRefObjectInfo()

{

 LPMODELDOC m\_ModelDoc
= NULL;

 HRESULT hres = NOERROR;

 //
Retrieve IModelDoc pointer

 hres = UserApp->getSWApp()->get\_IActiveDoc(
&m\_ModelDoc );

 if( m\_ModelDoc == NULL
)

  return;

long type;

// Helper function

IFeature\* m\_Feature = GetSelectedFeature( m\_ModelDoc,
&type );

if( m\_Feature != NULL )

{

BSTR bFeatName;

// Get feature name

hres = m\_Feature->get\_Name(
&bFeatName );

BSTR bTypeName;

// Get the feature type

hres = m\_Feature->GetTypeName(
&bTypeName );

CString featName( bFeatName
);

CString typeName( bTypeName
);

CString message;

// Display message to user

message.Format( \_T("Type:
%s\nName: %s"), typeName, featName );

SysFreeString(bFeatName);

SysFreeString(bTypeName);

// If the selected feature is a Reference Plane

if (type == swSelDATUMPLANES)

{

LPUNKNOWN iUnk = NULL;

//
Get the RefPlane interface

hres = m\_Feature->IGetSpecificFeature(
&iUnk );

IRefPlane\* refPlane = NULL;

hres = iUnk->QueryInterface(
IID\_IRefPlane, (LPVOID\*)&refPlane);

double values[9];

// Get Ref Plane parameters

hres = refPlane->IGetRefPlaneParams(
values );

CString message2;       //
Display message to user

message2.Format( \_T("RefPlaneParams\nOrigin:%f,
%f, %f\n X-Dir:%f, %f, %f\nNormal:%f, %f, %f"), values[0], values[1],
values[2], values[3], values[4], values[5], values[6], values[7], values[8]
);

AfxMessageBox( message2 );

refPlane->Release();

}

else if (type == swSelDATUMAXES)

// If the selected feature is a Reference Axis

{

LPUNKNOWN iUnk = NULL;

// Get the RefAxis interface

hres = m\_Feature->IGetSpecificFeature(
&iUnk );

IRefAxis\* refAxis = NULL;

hres = iUnk->QueryInterface(
IID\_IRefAxis, (LPVOID\*)&refAxis);

double values[6];

// Get Ref Axis parameters

hres = refAxis->IGetRefAxisParams(
values );

// Display message to user

CString message2;

message2.Format( \_T("RefPlaneParams\nStartPt:%f,
%f, %f\nEndPt:%f, %f, %f"), values[0], values[1], values[2], values[3],
values[4], values[5] );

AfxMessageBox( message2 );

refAxis->Release();

}

// Display message to user

AfxMessageBox( message );

}

m\_ModelDoc->Release();

m\_Feature->Release();

}