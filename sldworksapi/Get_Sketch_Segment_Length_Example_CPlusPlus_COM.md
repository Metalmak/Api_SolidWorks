<!-- source: sldworksapi/Get_Sketch_Segment_Length_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get Sketch Segment Length Example (C++ COM)

This example shows how to get the length of a sketch segment.

double GetLength(LPMODELDOC Part,LPSELECTIONMGR SelectionManager,LPTSTR
objectName)

{

LPTSTR segType = \_T("EXTSKETCHSEGMENT");

VARIANT\_BOOL success;

double Length(-1.0);  //
neg number == failure

Part->SelectByID(objectName,
segType, 0.0, 0.0, 0,&success);

if(Part->SelectByID(objectName,
segType, 0.0, 0.0, 0,&success) == S\_OK && success)

{

LPSKETCHSEGMENT SketchSegment;

LPDISPATCH disp;

if(SelectionManager->GetSelectedObject2(1,&disp)
== S\_OK &&

disp != NULL &&

disp->QueryInterface(IID\_ISketchSegment,(void
\*\*)&SketchSegment) == S\_OK &&

SketchSegment != NULL)

SketchSegment->GetLength(&Length);

}

return Length;

}