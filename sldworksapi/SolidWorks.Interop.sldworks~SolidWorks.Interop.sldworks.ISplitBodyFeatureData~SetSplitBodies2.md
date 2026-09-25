<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~SetSplitBodies2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSplitBodies2 Method (ISplitBodyFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISplitBodyFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData.html) : SetSplitBodies2 Method (ISplitBodyFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PathVar*
:   Array of paths and file names of the part documents to which to save the split bodies in this Split feature

*FlagVar*
:   Array of booleans indicating whether to consume each corresponding PathVar body; true to remove it from the original part, false to not

*BodyOrigin*
:   Array of sketch points, vertices, or reference points indicating the origins of each PathVar body; null elements are also permitted

Edits the current split bodies in this Split feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetSplitBodies2( _    ByVal PathVar As System.Object, _    ByVal FlagVar As System.Object, _    ByVal BodyOrigin As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISplitBodyFeatureData Dim PathVar As System.Object Dim FlagVar As System.Object Dim BodyOrigin As System.Object   instance.SetSplitBodies2(PathVar, FlagVar, BodyOrigin) ``` | |

| C# |  |
| --- | --- |
| ``` void SetSplitBodies2(     System.object PathVar,    System.object FlagVar,    System.object BodyOrigin ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetSplitBodies2(  &   System.Object^ PathVar, &   System.Object^ FlagVar, &   System.Object^ BodyOrigin ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PathVar*
:   Array of paths and file names of the part documents to which to save the split bodies in this Split feature

*FlagVar*
:   Array of booleans indicating whether to consume each corresponding PathVar body; true to remove it from the original part, false to not

*BodyOrigin*
:   Array of sketch points, vertices, or reference points indicating the origins of each PathVar body; null elements are also permitted

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SplitBodyFeatureData::SetSplitBodies2.

# ![](dotnetimages/collapse.gif)Remarks

Call this method after calling [ISplitBodyFeatureData::GetSplitBodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISplitBodyFeatureData~GetSplitBodies.html) or [ISplitBodyFeatureData::IGetSplitBodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISplitBodyFeatureData~IGetSplitBodies.html) to change which split bodies to include in this Split feature.

See Accessing Selections that Define Features for additional details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISplitBodyFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData.html)

[ISplitBodyFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData_members.html)

[IFeatureManager::PreSplitBody2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~PreSplitBody2.html)

[IFeatureManager::PostSplitBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~PostSplitBody.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0