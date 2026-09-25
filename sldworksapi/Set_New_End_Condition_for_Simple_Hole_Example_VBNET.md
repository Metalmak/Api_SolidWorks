<!-- source: sldworksapi/Set_New_End_Condition_for_Simple_Hole_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Set New End Condition for Simple Hole Feature Example (VB.NET)

This example shows how to set a new end condition for a simple hole
feature.

'----------------------------------------------------------------------------
' Preconditions:
' 1. Open a part document containing a block with a simple hole feature
named
'    **Hole1**.
' 2. Select the bottom face of the block.
' 3. Open the Immediate window.
'
' Postconditions:
' 1. Sets the bottom face of the block as the new end condition
'    of the simple hole feature.
' 2. Examine the Immediate window.
'----------------------------------------------------------------------------

Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
System.Runtime.InteropServices
Imports
System
Imports
System.Diagnostics

Partial
Class
SolidWorksMacro

    Dim
Model As
ModelDoc2
    Dim
SelMgr As
SelectionMgr
    Dim
SimpleHoleFeature As
Feature
    Dim
SimpleHoleFeature\_DEF As
SimpleHoleFeatureData2
    Dim
bottomFace As
Face2
    Dim
SimpleHoleEndCondition As
Face2
    Dim
boolstatus As
Boolean

    Sub
main()

        Model = swApp.**ActiveDoc**
        SelMgr = Model.**SelectionManager**

        bottomFace = SelMgr.**GetSelectedObject6**(1, -1)

        boolstatus = Model.**Extension**.**SelectByID2**("Hole1",
"BODYFEATURE",
0, 0, 0, False,
0, Nothing,
swSelectOption\_e.swSelectOptionDefault)
        SimpleHoleFeature = SelMgr.**GetSelectedObject6**(1, -1)

        SimpleHoleFeature\_DEF = SimpleHoleFeature.**GetDefinition**
        SimpleHoleFeature\_DEF.**AccessSelections**(Model,
Nothing)

        Dim
SimpleHoleType As
Integer

        '
Print the type of hole
        SimpleHoleType =
SimpleHoleFeature\_DEF.**Type**
        Debug.Print("Hole type: "
& SimpleHoleType)

        ' If the end condition is blind, no
reference is returned
        SimpleHoleEndCondition =
SimpleHoleFeature\_DEF.**GetEndConditionReference**(SimpleHoleType)

        SimpleHoleFeature\_DEF.**Type** = swEndConditions\_e.**swEndCondUpToSurface**
        SimpleHoleFeature\_DEF.**SetEndConditionReference**(bottomFace)
        SimpleHoleFeature.**ModifyDefinition**(SimpleHoleFeature\_DEF,
Model, Nothing)
        SimpleHoleFeature\_DEF.**AccessSelections**(Model,
Nothing)

        ' Print the type of hole
        SimpleHoleType =
SimpleHoleFeature\_DEF.**Type**
        Debug.Print("Hole type after
setting end condition: " & SimpleHoleType)

        ' The end condition is not blind,
so a reference is returned
        SimpleHoleEndCondition =
SimpleHoleFeature\_DEF.**GetEndConditionReference**(SimpleHoleType)

        SimpleHoleFeature\_DEF.**ReleaseSelectionAccess**()

    End
Sub

    Public
swApp As
SldWorks

End
Class