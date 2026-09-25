<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetDraftAngleReverseDirection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDraftAngleReverseDirection Method (IBoundaryBossFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBoundaryBossFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html) : GetDraftAngleReverseDirection Method (IBoundaryBossFeatureData) |

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

Gets whether the draft angle is flipped for the specified curve in the specified direction in this boundary feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDraftAngleReverseDirection( _    ByVal Direction As System.Integer, _    ByVal GuideIndex As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBoundaryBossFeatureData Dim Direction As System.Integer Dim GuideIndex As System.Integer Dim value As System.Boolean   value = instance.GetDraftAngleReverseDirection(Direction, GuideIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetDraftAngleReverseDirection(     System.int Direction,    System.int GuideIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetDraftAngleReverseDirection(  &   System.int Direction, &   System.int GuideIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Direction*
:   Direction as defined in swBoundaryBossDirection\_e

*GuideIndex*
:   Index of the curve (see **Remarks**)

#### Return Value

True if the draft angle is flipped, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BoundaryBossFeatureData::GetDraftAngleReverseDirection.

# ![](dotnetimages/collapse.gif)Example

[Insert Boundary Feature (C#)](Insert_Boundary_Feature_Example_CSharp.htm)

[Insert Boundary Feature (VB.NET)](Insert_Boundary_Feature_Example_VBNET.htm)

[Insert Boundary Feature (VBA)](Insert_Boundary_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [IBoundaryBossFeatureData::GetCurvesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetCurvesCount.html) to get a valid range of values for GuideIndex.

# ![](dotnetimages/collapse.gif)See Also

####

[IBoundaryBossFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html)

[IBoundaryBossFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData_members.html)

[IBoundaryBossFeatureData::GetDraftAngle Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetDraftAngle.html)

[IBoundaryBossFeatureData::SetDraftAngle Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetDraftAngle.html)

[IBoundaryBossFeatureData::SetDraftAngleReverseDirection Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetDraftAngleReverseDirection.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0