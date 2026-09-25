<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~SetEntitiesWeldPath.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetEntitiesWeldPath Method (ICosmeticWeldBeadFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICosmeticWeldBeadFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData.html) : SetEntitiesWeldPath Method (ICosmeticWeldBeadFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Entities*
:   Array of entities of [edges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html), [sketches](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html), or a combination of edges and sketches (see **Remarks**)

Sets the entities for this cosmetic weld bead, which was created using a weld path.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetEntitiesWeldPath( _    ByVal Entities As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICosmeticWeldBeadFeatureData Dim Entities As System.Object   instance.SetEntitiesWeldPath(Entities) ``` | |

| C# |  |
| --- | --- |
| ``` void SetEntitiesWeldPath(     System.object Entities ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetEntitiesWeldPath(  &   System.Object^ Entities ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Entities*
:   Array of entities of [edges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html), [sketches](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html), or a combination of edges and sketches (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CosmeticWeldBeadFeatureData::SetEntitiesWeldPath.

# ![](dotnetimages/collapse.gif)See Also

####

[ICosmeticWeldBeadFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData.html)

[ICosmeticWeldBeadFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData_members.html)

[ICosmeticWeldBeadFeatureData::GetEntitiesWeldPath](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GetEntitiesWeldPath.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0