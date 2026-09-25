<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetReactionForcesAndMomentsWithSelections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetReactionForcesAndMomentsWithSelections Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetReactionForcesAndMomentsWithSelections Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NStepNumber*
:   Solution step number (use 1 for static)

*DispPlane*
:   Plane, axis, or coodinate system relative to which to list reaction results

*NUnits*
:   Unit as defined in [swsForceUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsForceUnit_e.html)

*SelectedObjects*
:   Array of entities for which to get reaction results

*SelectionAndEntireModelReactionForcesAndMoments*
:   Array of reaction forces and moments for the selected entities and the entire model (see **Remarks**)

*EachSelectedObjectReactionForcesAndMoments*
:   Array of reaction forces and moments for each selected entity (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the reaction forces and moments for selections and the entire model at the specified solution step.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetReactionForcesAndMomentsWithSelections( _    ByVal NStepNumber As System.Integer, _    ByVal DispPlane As System.Object, _    ByVal NUnits As System.Integer, _    ByVal SelectedObjects As System.Object, _    ByRef SelectionAndEntireModelReactionForcesAndMoments As System.Object, _    ByRef EachSelectedObjectReactionForcesAndMoments As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NStepNumber As System.Integer Dim DispPlane As System.Object Dim NUnits As System.Integer Dim SelectedObjects As System.Object Dim SelectionAndEntireModelReactionForcesAndMoments As System.Object Dim EachSelectedObjectReactionForcesAndMoments As System.Object Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetReactionForcesAndMomentsWithSelections(NStepNumber, DispPlane, NUnits, SelectedObjects, SelectionAndEntireModelReactionForcesAndMoments, EachSelectedObjectReactionForcesAndMoments, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetReactionForcesAndMomentsWithSelections(     System.int NStepNumber,    System.object DispPlane,    System.int NUnits,    System.object SelectedObjects,    out System.object SelectionAndEntireModelReactionForcesAndMoments,    out System.object EachSelectedObjectReactionForcesAndMoments,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetReactionForcesAndMomentsWithSelections(  &   System.int NStepNumber, &   System.Object^ DispPlane, &   System.int NUnits, &   System.Object^ SelectedObjects, &   [Out] System.Object^ SelectionAndEntireModelReactionForcesAndMoments, &   [Out] System.Object^ EachSelectedObjectReactionForcesAndMoments, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NStepNumber*
:   Solution step number (use 1 for static)

*DispPlane*
:   Plane, axis, or coodinate system relative to which to list reaction results

*NUnits*
:   Unit as defined in [swsForceUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsForceUnit_e.html)

*SelectedObjects*
:   Array of entities for which to get reaction results

*SelectionAndEntireModelReactionForcesAndMoments*
:   Array of reaction forces and moments for the selected entities and the entire model (see **Remarks**)

*EachSelectedObjectReactionForcesAndMoments*
:   Array of reaction forces and moments for each selected entity (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array of reaction forces and moments (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetReactionForcesAndMomentsWithSelections.

# ![](dotnetimages/collapse.gif)Example

[Create Linear Dynamic Study (VBA)](Create_Dynamic_Harmonic_Study_Example_VB.htm)

[Create Linear Dynamic Study (VB.NET)](Create_Dynamic_Harmonic_Study_Example_VBNET.htm)

[Create Linear Dynamic Study (C#)](Create_Dynamic_Harmonic_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for static, nonlinear, drop test, and dynamic studies.

SelectionAndEntireModelReactionForcesAndMoments array contains 16 elements:

{

*summation\_xcoord\_forces\_all\_selections,*

*summation\_ycoord\_forces\_all\_selections,*

*summation\_zcoord\_forces\_all\_selections,*

*resultant\_force\_all\_selections*,

*summation\_xcoord\_moments\_all\_selections,*

*summation\_ycoord\_moments\_all\_selections,*

*summation\_zcoord\_moments\_all\_selections,*

*resultant\_moment\_all\_selections*,

*summation\_xcoord\_forces\_entire\_model,*

**summation\_ycoord\_forces\_entire\_model,**

*summation\_zcoord\_forces\_entire\_model,*

*resultant\_force\_entire\_model*,

*summation\_xcoord\_moments\_entire\_model,*

*summation\_ycoord\_moments\_entire\_model,*

*summation\_zcoord\_moments\_entire\_model,*

*resultant\_moment\_entire\_model*

*}*

EachSelectedObjectReactionForcesAndMoments array contains (8 X *no\_of\_selections*) elements:

{

*selection\_1\_xcoord\_reaction\_force,*

*selection\_1\_ycoord\_reaction\_force,*

*selection\_1\_zcoord\_reaction\_force,*

*selection\_1\_resultant\_reaction\_force*,

*selection\_1\_xcoord\_reaction\_moment,*

*selection\_1\_ycoord\_reaction\_moment,*

*selection\_1\_zcoord\_reaction\_moment,*

*selection\_1\_resultant\_reaction\_moment,*

*...*

**selection\_n\_xcoord\_reaction\_force,**

***selection\_n\_ycoord\_reaction\_force,*

*selection\_n\_zcoord\_reaction\_force,*

*selection\_n\_resultant\_reaction\_force*,

*selection\_n\_xcoord\_reaction\_moment,*

*selection\_n\_ycoord\_reaction\_moment,*

*selection\_n\_zcoord\_reaction\_moment,*

*selection\_n\_resultant\_reaction\_moment***

*}*

This method returns the reaction forces and moments at each node of the entire model:

{

*node\_1*,

*node\_1\_xcoord\_reaction\_force,*

*node\_1\_ycoord\_reaction\_force,*

*node\_1\_zcoord\_reaction\_force,*

*node\_1\_resultant\_reaction\_force*,

*node\_1\_xcoord\_reaction\_moment,*

*node\_1\_ycoord\_reaction\_moment,*

*node\_1\_zcoord\_reaction\_moment,*

*node\_1\_resultant\_reaction\_moment*,

     ...

*node\_n*,

*node\_n\_xcoord\_reaction\_force,*

*node\_n\_ycoord\_reaction\_force,*

*node\_n\_zcoord\_reaction\_force,*

*node\_n\_resultant\_reaction\_force*,

*node\_n\_xcoord\_reaction\_moment,*

*node\_n\_ycoord\_reaction\_moment,*

*node\_n\_zcoord\_reaction\_moment,*

*node\_n\_resultant\_reaction\_moment*

}

In all of the arrays, the nodes are integers, and the reaction forces and moments are in decimal or scientific notation.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetDisplacementComponentForAllStepsAtNode Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDisplacementComponentForAllStepsAtNode.html)

[ICWResults::GetDisplacementForEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDisplacementForEntities.html)

[ICWResults::GetMinMaxDisplacement Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxDisplacement.html)

[ICWResults::GetRotationalDisplacement Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetRotationalDisplacement.html)

[ICWResults::GetTranslationalDisplacement Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetTranslationalDisplacement.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0