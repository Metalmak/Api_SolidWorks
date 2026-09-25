<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~InsertEntity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| InsertEntity Method (ICWRestraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html) : InsertEntity Method (ICWRestraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Face, edge, or vertex

Inserts an entity in the restraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertEntity( _    ByVal DispEntity As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRestraint Dim DispEntity As System.Object   instance.InsertEntity(DispEntity) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertEntity(     System.object DispEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertEntity(  &   System.Object^ DispEntity ) ``` | |

#### Parameters

*DispEntity*
:   Face, edge, or vertex

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRestraint::InsertEntity.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

[ICWRestraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint_members.html)

[ICWRestraint::RemoveEntity Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~RemoveEntity.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0