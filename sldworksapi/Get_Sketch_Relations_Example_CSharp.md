<!-- source: sldworksapi/Get_Sketch_Relations_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Get Sketch Relations Example (C#)

This example shows how to get all of the sketch relations in a sketch.

//------------------------------------------------------------------
// Preconditions:
// 1. Open a part or assembly document.
// 2. Select the sketch whose relations you want to see.
//
// Postconditions: Inspect the Immediate window.
//--------------------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
using
System;
using
System.Diagnostics;
namespace
GetDefinitionEntities2\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        public
void Main()
    {
        ModelDoc2
swModel = default(ModelDoc2);
        SelectionMgr
swSelMgr = default(SelectionMgr);
        SelectData
swSelData = default(SelectData);
        Feature
swFeat = default(Feature);
        Sketch
swSketch = default(Sketch);
        SketchRelationManager
swSkRelMgr = default(SketchRelationManager);
        SketchRelation
swSkRel = default(SketchRelation);

DisplayDimension
dispDim = default(DisplayDimension);
        object[]
vSkRelArr = null;
        int[]
vEntTypeArr = null;
        object[]
vEntArr = null;
        object[]
vDefEntArr = null;
        SketchSegment
swSkSeg = default(SketchSegment);
        SketchPoint
swSkPt = default(SketchPoint);
        int
i = 0;
        int
j = 0;
        bool
bRet = false;

        swModel = (ModelDoc2)swApp.**ActiveDoc**;
        swSelMgr = (SelectionMgr)swModel.**SelectionManager**;
        swSelData = (SelectData)swSelMgr.**CreateSelectData**();
        swFeat = (Feature)swSelMgr.**GetSelectedObject6**(1,
-1);
        swSketch = (Sketch)swFeat.**GetSpecificFeature2**();
        swSkRelMgr = swSketch.**RelationManager**;

        swModel.**ClearSelection2**(true);

        Debug.Print("File
= " + swModel.**GetPathName**());
        Debug.Print("  Feat
= " + swFeat.**Name**);

        vSkRelArr = (object[])swSkRelMgr.**GetRelations**((int)swSketchRelationFilterType\_e.swAll);
        if
((vSkRelArr == null))
            return;
        foreach
( SketchRelation
vRel in
vSkRelArr) {
            swSkRel = (SketchRelation)vRel;

            Debug.Print("    Relation("
+ i + ")");
            Debug.Print("      Type
= " + swSkRel.**GetRelationType**());

            dispDim =
(DisplayDimension)swSkRel.**GetDisplayDimension**();
            if
(dispDim != null)
{
                Debug.Print("      Display
dimension
= " + dispDim.**GetNameforSelection**());
            }

            vEntTypeArr = (int[])swSkRel.**GetEntitiesType**();
            vEntArr = (object[])swSkRel.**GetEntities**();

            vDefEntArr = (object[])swSkRel.**GetDefinitionEntities2**();
            if
((vDefEntArr == null))
{
            } else
{
                Debug.Print("    Number
of definition entities in this relation: "
+ vDefEntArr.GetUpperBound(0));
            }

            if
((vEntTypeArr != null)
& (vEntArr != null))
{

                if
(vEntTypeArr.GetUpperBound(0) == vEntArr.GetUpperBound(0)) {
                    j = 0;

                    foreach
( swSketchRelationEntityTypes\_e
vType in
vEntTypeArr) {
                        Debug.Print("        EntType    =
" + vType);

                        switch
(vType) {
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Unknown:
                                Debug.Print("          Not
known");

                                break;
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_SubSketch:
                                Debug.Print("SubSketch");

                                break;
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Point:
                                swSkPt = (SketchPoint)vEntArr[j];
                                Debug.Assert((swSkPt
!= null));

                                Debug.Print("          SkPoint
ID = [" + ((int[])(swSkPt.**GetID**()))[0]
+ ", " +
((int[])(swSkPt.**GetID**()))[1]
+ "]");

                                bRet = swSkPt.**Select4**(true,
swSelData);
                                //
                                break;

                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Line:
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Arc:
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Ellipse:
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Parabola:
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Spline:

                                swSkSeg = (SketchSegment)vEntArr[j];

                                Debug.Print("          SkSeg
ID = [" + ((int[])(swSkSeg.**GetID**()))[0]
+ ", " +
((int[])(swSkSeg.**GetID**()))[1]
+ "]");

                                bRet = swSkSeg.**Select4**(true,
swSelData);

                                break;
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Hatch:
                                Debug.Print("Hatch");

                                break;
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Text:
                                Debug.Print("Text");

                                break;
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Plane:
                                Debug.Print("Plane");

                                break;
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Cylinder:
                                Debug.Print("Cylinder");

                                break;
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Sphere:
                                Debug.Print("Sphere");

                                break;
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Surface:
                                Debug.Print("Surface");

                                break;
                            case
swSketchRelationEntityTypes\_e.swSketchRelationEntityType\_Dimension:
                                Debug.Print("Dimension");

                                break;
                            default:
                                Debug.Print("Something
else");

                                break;
                        }

                        j = j + 1;

                    }
                }
            }

            i = i + 1;

        }

    }

        public
SldWorks
swApp;

    }

}