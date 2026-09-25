<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetGuideTangencyType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetGuideTangencyType Method (IBoundaryBossFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBoundaryBossFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html) : SetGuideTangencyType Method (IBoundaryBossFeatureData) |

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

*TangType*
:   Type of tangency as defined in swBoundaryBossTangencyType\_e

Sets the type of tangency for the specified curve in the specified direction in this boundary feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetGuideTangencyType( _    ByVal Direction As System.Integer, _    ByVal GuideIndex As System.Integer, _    ByVal TangType As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBoundaryBossFeatureData Dim Direction As System.Integer Dim GuideIndex As System.Integer Dim TangType As System.Integer   instance.SetGuideTangencyType(Direction, GuideIndex, TangType) ``` | |

| C# |  |
| --- | --- |
| ``` void SetGuideTangencyType(     System.int Direction,    System.int GuideIndex,    System.int TangType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetGuideTangencyType(  &   System.int Direction, &   System.int GuideIndex, &   System.int TangType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Direction*
:   Direction as defined in swBoundaryBossDirection\_e

*GuideIndex*
:   Index of the curve (see **Remarks**)

*TangType*
:   Type of tangency as defined in swBoundaryBossTangencyType\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BoundaryBossFeatureData::SetGuideTangencyType.

# ![](dotnetimages/collapse.gif)Remarks

This method is only available when a minimum of three curves in the specified direction exist.

Call [IBoundaryBossFeatureData::GetCurvesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetCurvesCount.html) to get a valid range of values for GuideIndex.

| If specified curve is... | Then the valid types of tangency as defined in swBoundaryBossTangencyType\_e are... |
| --- | --- |
| [Sketch curve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) | * swBoundaryBossTangency\_None* swBoundaryBossTangency\_DirectionVector* swBoundaryBossTangency\_NormalToProfile |
| [Face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) | * swBoundaryBossTangency\_None* swBoundaryBossTangency\_DirectionVector* swBoundaryBossTangency\_NormalToProfile* swBoundaryBossTangency\_TangencyToFace* swBoundaryBossTangency\_CurvatureToFace |
| [Edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html) | * swBoundaryBossTangency\_Default* swBoundaryBossTangency\_None* swBoundaryBossTangency\_DirectionVector* swBoundaryBossTangency\_TangencyToFace* swBoundaryBossTangency\_CurvatureToFace |

# ![](dotnetimages/collapse.gif)See Also

####

[IBoundaryBossFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html)

[IBoundaryBossFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData_members.html)

[IBoundaryBossFeatureData::GetGuideTangencyType Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetGuideTangencyType.html)

[IBoundaryBossFeatureData::GetTangentApplyToAll Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetTangentApplyToAll.html)

[IBoundaryBossFeatureData::GetTangentDirectionReversed Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetTangentDirectionReversed.html)

[IBoundaryBossFeatureData::GetTangentInfluence Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetTangentInfluence.html)

[IBoundaryBossFeatureData::GetTangentLength Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetTangentLength.html)

[IBoundaryBossFeatureData::SetTangentApplyToAll Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetTangentApplyToAll.html)

[IBoundaryBossFeatureData::SetTangentDirectionReversed Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetTangentDirectionReversed.html)

[IBoundaryBossFeatureData::SetTangentInfluence Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetTangentInfluence.html)

[IBoundaryBossFeatureData::SetTangentLength Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetTangentLength.html)

[IBoundaryBossFeatureData::MergeTangentFaces Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~MergeTangentFaces.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0