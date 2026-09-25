<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~SetReferenceEntity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetReferenceEntity Method (ICWGravity) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWGravity Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity.html) : SetReferenceEntity Method (ICWGravity) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RefEntity*
:   Face, edge, or plane

Sets the direction reference for gravity.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetReferenceEntity( _    ByVal RefEntity As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWGravity Dim RefEntity As System.Object   instance.SetReferenceEntity(RefEntity) ``` | |

| C# |  |
| --- | --- |
| ``` void SetReferenceEntity(     System.object RefEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetReferenceEntity(  &   System.Object^ RefEntity ) ``` | |

#### Parameters

*RefEntity*
:   Face, edge, or plane

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWGravity::SetReferenceEntity.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWGravity Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity.html)

[ICWGravity Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity_members.html)

[ICWGravity::ReverseDirectionAlongPlaneDir1 Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionAlongPlaneDir1.html)

[ICWGravity::ReverseDirectionAlongPlaneDir2 Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionAlongPlaneDir2.html)

[ICWGravity::ReverseDirectionNormalToPlane Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionNormalToPlane.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0