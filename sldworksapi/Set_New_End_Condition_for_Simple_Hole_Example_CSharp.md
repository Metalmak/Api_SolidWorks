<!-- source: sldworksapi/Set_New_End_Condition_for_Simple_Hole_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Set New End Condition for Simple Hole Feature Example (C#)

This example shows how to set a new end condition for a simple hole
feature.

//----------------------------------------------------------------------------
// Preconditions:
// 1. Open a part document containing a block with a simple hole feature
named
/     **Hole1**.
// 2. Select the bottom face of the block.
// 3. Open the Immediate window.
//
// Postconditions:
// 1. Sets the bottom face of the block as the new end condition
//    of the simple hole feature.
// 2. Examine the Immediate window.
//----------------------------------------------------------------------------
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
SimpleHoleFeatureData\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        ModelDoc2
Model;
        SelectionMgr
SelMgr;
        Feature
SimpleHoleFeature;
        SimpleHoleFeatureData2
SimpleHoleFeature\_DEF;
        Face2
bottomFace;
        Face2
SimpleHoleEndCondition;

        bool
boolstatus;

        public
void Main()
        {
            Model = (ModelDoc2)swApp.**ActiveDoc**;
            SelMgr = (SelectionMgr)Model.**SelectionManager**;

            bottomFace = (Face2)SelMgr.**GetSelectedObject6**(1,
-1);

            boolstatus = Model.**Extension**.**SelectByID2**("Hole1",
"BODYFEATURE",
0, 0, 0, false,
0, null, (int)swSelectOption\_e.swSelectOptionDefault);
            SimpleHoleFeature = (Feature)SelMgr.**GetSelectedObject6**(1,
-1);

            SimpleHoleFeature\_DEF = (SimpleHoleFeatureData2)SimpleHoleFeature.**GetDefinition**();
            SimpleHoleFeature\_DEF.**AccessSelections**(Model,
null);

            int
SimpleHoleType = 0;

            // Print the type of hole
            SimpleHoleType =
SimpleHoleFeature\_DEF.**Type**;
            Debug.Print("Hole
type: " + SimpleHoleType);

            // If the end condition is
blind, no reference is returned
            SimpleHoleEndCondition = (Face2)SimpleHoleFeature\_DEF.**GetEndConditionReference**(out
SimpleHoleType);

            SimpleHoleFeature\_DEF.**Type** = (int)swEndConditions\_e.swEndCondUpToSurface;
            SimpleHoleFeature\_DEF.**SetEndConditionReference**(bottomFace);
            SimpleHoleFeature.**ModifyDefinition**(SimpleHoleFeature\_DEF,
Model, null);
            SimpleHoleFeature\_DEF.**AccessSelections**(Model,
null);

            // Print the type of hole
            SimpleHoleType =
SimpleHoleFeature\_DEF.**Type**;
            Debug.Print("Hole
type after setting end condition: " +
SimpleHoleType);

            // The end condition is not
blind, so a reference is returned
            SimpleHoleEndCondition = (Face2)SimpleHoleFeature\_DEF.**GetEndConditionReference**(out
SimpleHoleType);
            Debug.Print("End
condition face ID: " +
SimpleHoleEndCondition.**GetFaceId**());

            SimpleHoleFeature\_DEF.**ReleaseSelectionAccess**();

        }

        public
SldWorks
swApp;

    }
}