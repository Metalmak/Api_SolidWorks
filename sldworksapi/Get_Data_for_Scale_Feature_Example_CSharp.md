<!-- source: sldworksapi/Get_Data_for_Scale_Feature_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Get Data for Scale Feature Example (C#)

This example shows how to get the data for the selected scale feature.

//----------------------------------------------------------------------------
// Preconditions:
// 1. Open a model document with a scale feature.
// 2. Select the scale feature.
//
// Postconditions: Inspect the Immediate window.
//---------------------------------------------------------------------------
using
Microsoft.VisualBasic;
using
System;
using
System.Collections;
using
System.Collections.Generic;
using
System.Data;
using
System.Diagnostics;
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
namespace
ScaleFeatureData\_CSharp.csproj
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
            Feature
swFeat = default(Feature);
            ScaleFeatureData
swScale = default(ScaleFeatureData);
            Feature
swCoordSys = default(Feature);
            double
nX\_Scale = 0;
            double
nY\_Scale = 0;
            double
nZ\_scale = 0;
            bool
bIsUniform = false;

            swModel = (ModelDoc2)swApp.**ActiveDoc**;
            swSelMgr = (SelectionMgr)swModel.**SelectionManager**;
            swFeat = (Feature)swSelMgr.**GetSelectedObject6**(1,
-1);
            swScale = (ScaleFeatureData)swFeat.**GetDefinition**();
            swCoordSys = (Feature)swScale.**CoordinateSystem**;

            swScale.**GetScale**(out
nX\_Scale, out
nY\_Scale, out
nZ\_scale, out
bIsUniform);

            Debug.Print("File
= " + swModel.**GetPathName**());
            Debug.Print("Feature
= " + swFeat.**Name**);
            Debug.Print("
X scaling factor = " + nX\_Scale);
            Debug.Print("
Y scaling factor = " + nY\_Scale);
            Debug.Print("
Z scaling factor = " + nZ\_scale);
            Debug.Print("
Is uniform = " + bIsUniform);
            Debug.Print("
Scaling type as defined in swScaleType\_e = "
+ swScale.**Type**);
            Debug.Print("
Bodies count = " + swScale.**GetBodiesCount**());
            Debug.Print("
Is uniform = " + swScale.**IsUniform**);
            Debug.Print("
Uniform scaling factor = " + swScale.**ScaleUniform**);
            Debug.Print("
X scaling factor = " + swScale.**ScaleX**);
            Debug.Print("
Y scaling factor = " + swScale.**ScaleY**);
            Debug.Print("
Z scaling factor = " + swScale.**ScaleZ**);

            if
((swCoordSys != null))
            {
                Debug.Print("
CoorSys = " + swCoordSys.**Name**);
            }
        }

        public
SldWorks
swApp;

    }

}