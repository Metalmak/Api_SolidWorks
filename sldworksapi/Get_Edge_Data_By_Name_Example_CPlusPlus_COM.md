<!-- source: sldworksapi/Get_Edge_Data_By_Name_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get Edge Data By Name Example (C++ COM)

This example shows how to get an edge by its
name and then get the underlying curve parameters and curve length. Import swconst.tlb.

IEdge::IGetCurveParams2 returns an array, so
this code must be used in an in-process DLL. Otherwise, use IEdge::GetCurveParams2
that returns a VARIANT.

void GetEdgeData(ISldWorks\* m\_pSldWorks)

{

 HRESULT
res = NOERROR;

 LPMODELDOC2
p\_ModelDoc = NULL;

 LPPARTDOC
p\_PartDoc = NULL;

 LPENTITY
p\_Entity = NULL;

 long
doctype;

 //
Retrieve the model document pointer

 res
= m\_pSldWorks->get\_IActiveDoc2(
&p\_ModelDoc );

 if(
res != S\_OK || p\_ModelDoc == NULL ) return;

 res
= p\_ModelDoc->GetType(&doctype);

 if
(doctype != swDocPART )return;

 res
= p\_ModelDoc->QueryInterface(IID\_IPartDoc, (LPVOID \*)&p\_PartDoc);

 res
= p\_ModelDoc->GetType(&doctype);

 if
(doctype != swDocPART )return;

 //
Get an entity by its name "FredsEdge"

 res
= p\_PartDoc->IGetEntityByName(\_T("FredsEdge"),
swSelEDGES, &p\_Entity);

 if
(res == S\_OK && p\_Entity != NULL)// If entity was found successfully

 {

  LPEDGE
p\_Edge = NULL;  //
See if Entity is an Edge

  res
= p\_Entity->QueryInterface( IID\_IEdge, (LPVOID\*)&p\_Edge);

  if
(res == S\_OK && p\_Edge != NULL) // If Entity is an Edge

  {

   LPCURVE
p\_Curve;

   //
Get the edge's underlying curve

   res
= p\_Edge->IGetCurve(&p\_Curve);

   //
Since we do not keep the curve parameters with every edge, this call is
required or else the underlying curve parameters will be unknown.

   double
edgeData[10]={NULL};

   //
Get Edge data

   res
= p\_Edge->IGetCurveParams2(&edgeData[0]);

   //
Setup for ints packed into doubles

    union
PackedInts

   {

    double
value;

    int
intData[2];

   }
packedIntData;

   //
Get the integers from the double

   packedIntData.value
= edgeData[8];

   int
Notused = packedIntData.intData[0];

   int
curveType = packedIntData.intData[1];

   //
Get the integers from the double

   packedIntData.value
= edgeData[9];        int
Notused2 = packedIntData.intData[0];

   int
curveTag = packedIntData.intData[1];

   CString
message = \_T("Attribute is on Edge with:\n");

message.Format(\_T("\tStartPt = \t%lf \t%lf \t%lf
\n \tEndPt  =
\t%lf \t%lf \t%lf \n\tParams = \t%lf \t%lf \n\tCurveType = \t%i \n\tCurveTag
= \t%i"),

     edgeData[0],
edgeData[1], edgeData[2],

     edgeData[3],
edgeData[4], edgeData[5],

     edgeData[6],
edgeData[7],

     curveType,
curveTag);

   AfxMessageBox(
message );

   //
Get the length of the underlying curve

   double
curveLength;

   res
= p\_Curve->GetLength(edgeData[6],
edgeData[7],

&curveLength);

   message
= \_T("The Edge length is:\n");

   message.Format(\_T("\t%lf"),
curveLength);

   AfxMessageBox(
message );

   p\_Curve->Release();

  //
End if we got the Edge object

  }

  p\_Edge->Release();

  p\_Entity->Release();

 //
End if we got the Entity by its name

 }

 p\_PartDoc->Release();

 p\_ModelDoc->Release();

// End of function

}