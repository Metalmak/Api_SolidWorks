<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetDirectionVector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDirectionVector Method (IBoundaryBossFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBoundaryBossFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html) : GetDirectionVector Method (IBoundaryBossFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Direction*
:   Direction as defined in swBoundaryBossDirection\_e

*GuideIndex*
:   Index of the curve (see **Remarks**)

Gets the entity used as the direction vector for the specified curve in the specified direction in this boundary feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDirectionVector( _    ByVal Direction As System.Integer, _    ByVal GuideIndex As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBoundaryBossFeatureData Dim Direction As System.Integer Dim GuideIndex As System.Integer Dim value As System.Object   value = instance.GetDirectionVector(Direction, GuideIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetDirectionVector(     System.int Direction,    System.int GuideIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetDirectionVector(  &   System.int Direction, &   System.int GuideIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Direction*
:   Direction as defined in swBoundaryBossDirection\_e

*GuideIndex*
:   Index of the curve (see **Remarks**)

#### Return Value

Entity used as the direction vector:

* linear [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html)* [axis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)* [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)* [plane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BoundaryBossFeatureData::GetDirectionVector.

# ![](dotnetimages/collapse.gif)Example

[Insert Boundary Feature (C#)](Insert_Boundary_Feature_Example_CSharp.htm)

[Insert Boundary Feature (VB.NET)](Insert_Boundary_Feature_Example_VBNET.htm)

[Insert Boundary Feature (VBA)](Insert_Boundary_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is only available if the type of tangency of the direction vector is swBoundaryBossTangencyType\_e.swBoundaryBossTangency\_DirectionVector. Use [IBoundaryBossFeatureData::GetGuideTangencyType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetGuideTangencyType.html) to determine the type of tangency.

Call [IBoundaryBossFeatureData::GetCurvesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetCurvesCount.html) to get a valid range of values for GuideIndex.

**NOTE:** Using two vertices for the direction vector is not currently supported by the SOLIDWORKS API.

# ![](dotnetimages/collapse.gif)See Also

####

[IBoundaryBossFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html)

[IBoundaryBossFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData_members.html)

[IBoundaryBossFeatureData::SetDirectionVector Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetDirectionVector.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0