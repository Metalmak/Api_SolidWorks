<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetFreeBodyForcesAndMoments.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetFreeBodyForcesAndMoments Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetFreeBodyForcesAndMoments Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispPlane*
:   Plane, axis, or coordinate system relative to which the results are listed

*SelectedRefPoint*
:   Reference point used to list the moments for the forces that are available in ArraySelectedEntities; NULL to not list the moments

*ArraySelectedEntities*
:   Selected faces, edges, vertices, and components

*NUnits*
:   Output units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the x-, y-, and z-component and resultant free body forces and moments for the specified entities and the entire model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFreeBodyForcesAndMoments( _    ByVal DispPlane As System.Object, _    ByVal SelectedRefPoint As System.Object, _    ByVal ArraySelectedEntities As System.Object, _    ByVal NUnits As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim DispPlane As System.Object Dim SelectedRefPoint As System.Object Dim ArraySelectedEntities As System.Object Dim NUnits As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetFreeBodyForcesAndMoments(DispPlane, SelectedRefPoint, ArraySelectedEntities, NUnits, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetFreeBodyForcesAndMoments(     System.object DispPlane,    System.object SelectedRefPoint,    System.object ArraySelectedEntities,    System.int NUnits,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetFreeBodyForcesAndMoments(  &   System.Object^ DispPlane, &   System.Object^ SelectedRefPoint, &   System.Object^ ArraySelectedEntities, &   System.int NUnits, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*DispPlane*
:   Plane, axis, or coordinate system relative to which the results are listed

*SelectedRefPoint*
:   Reference point used to list the moments for the forces that are available in ArraySelectedEntities; NULL to not list the moments

*ArraySelectedEntities*
:   Selected faces, edges, vertices, and components

*NUnits*
:   Output units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

If SelectedRefPoint is NULL:

Array of eight doubles of the free body forces for all selections in ArraySelectedEntities and for the entire model:

* Summation of x-components of free body force for all selections* Summation of y-components of free body force for all selections* Summation of z-components of free body force for all selections* Resultant free body force for all selections* Summation of x-components of free body moment for the entire model* Summation of y-components of free body moment for the entire model* Summation of z-components of free body moment for the entire model* Resultant free body moment for the entire model

If SelectedRefPoint is not NULL:

Array of sixteen doubles of the free body forces and moments for all selections in ArraySelectedEntities and for the entire model:

* Summation of x-components of free body force for all selections* Summation of y-components of free body force for all selections* Summation of z-components of free body force for all selections* Resultant free body force for all selections* Summation of x-components of free body moment for all selections* Summation of y-components of free body moment for all selections* Summation of z-components of free body moment for all selections* Resultant free body moment for all selections* Summation of x-components of free body force for the entire model* Summation of y-components of free body force for the entire model* Summation of z-components of free body force for the entire model* Resultant free body force for the entire model* Summation of x-components of free body moment for the entire model* Summation of y-components of free body moment for the entire model* Summation of z-components of free body moment for the entire model* Resultant free body moment for the entire model

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetFreeBodyForcesAndMoments.

# ![](dotnetimages/collapse.gif)Example

[Get Free Body Forces and Moments (VBA)](Get_Free_Body_Forces_and_Moments_Example_VB.htm)

[Get Free Body Forces and Moments (VB.NET)](Get_Free_Body_Forces_and_Moments_Example_VBNET.htm)

[Get Free Body Forces and Moments (C#)](Get_Free_Body_Forces_and_Moments_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetFreeBodyForcesAndMomentsForAStep Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetFreeBodyForcesAndMomentsForAStep.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2013 SP0