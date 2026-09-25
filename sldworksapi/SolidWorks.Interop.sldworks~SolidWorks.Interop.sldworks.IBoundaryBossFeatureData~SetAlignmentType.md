<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetAlignmentType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetAlignmentType Method (IBoundaryBossFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBoundaryBossFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html) : SetAlignmentType Method (IBoundaryBossFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Direction*
:   Direction as defined in swBoundaryBossDirection\_e

*GuideIndex*
:   Index of the curve (see **Remarks**)

*AlignmentType*
:   Type of alignment as defined in swBoundaryBossAlignment\_e

Sets the type of alignment for the specified curve in the specified direction for this boundary feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetAlignmentType( _    ByVal Direction As System.Integer, _    ByVal GuideIndex As System.Integer, _    ByVal AlignmentType As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBoundaryBossFeatureData Dim Direction As System.Integer Dim GuideIndex As System.Integer Dim AlignmentType As System.Integer   instance.SetAlignmentType(Direction, GuideIndex, AlignmentType) ``` | |

| C# |  |
| --- | --- |
| ``` void SetAlignmentType(     System.int Direction,    System.int GuideIndex,    System.int AlignmentType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetAlignmentType(  &   System.int Direction, &   System.int GuideIndex, &   System.int AlignmentType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Direction*
:   Direction as defined in swBoundaryBossDirection\_e

*GuideIndex*
:   Index of the curve (see **Remarks**)

*AlignmentType*
:   Type of alignment as defined in swBoundaryBossAlignment\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BoundaryBossFeatureData::SetAlignmentType.

# ![](dotnetimages/collapse.gif)Remarks

This method is only available for a single-direction boundary feature.

You must use the appropriate combination of tangents and alignments.

| Type of [tangency](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetGuideTangencyType.html) as defined in swBoundaryBossTangencyType\_e | Type of alignment as defined in swBoundaryBossAlignment\_e |
| --- | --- |
| swBoundaryBossTangency\_DirectionVector  - or -  swBoundaryBossTangency\_NormalToProfile | * swAlignWithNextSection* swAlignWithSectionNormal |
| swBoundaryBossTangency\_TangencyToFace  -or -  swBoundaryBossTangency\_CurvatureToFace | * swAlignWithNextSection* swAlignWithSectionNormal* swAlignWithIsoParameter* swAlignWithOtherGeometry |

Call [IBoundaryBossFeatureData::GetCurvesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetCurvesCount.html) to get a valid range of values for GuideIndex.

# ![](dotnetimages/collapse.gif)See Also

####

[IBoundaryBossFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html)

[IBoundaryBossFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData_members.html)

[IBoundaryBossFeatureData::GetAlignmentType Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetAlignmentType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0