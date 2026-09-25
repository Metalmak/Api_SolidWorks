<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~RemoveEntity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| RemoveEntity Method (ICWRestraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html) : RemoveEntity Method (ICWRestraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIndex*
:   0-based index of the entity to remove

Removes the entity at the specified index from the restraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub RemoveEntity( _    ByVal NIndex As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRestraint Dim NIndex As System.Integer   instance.RemoveEntity(NIndex) ``` | |

| C# |  |
| --- | --- |
| ``` void RemoveEntity(     System.int NIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RemoveEntity(  &   System.int NIndex ) ``` | |

#### Parameters

*NIndex*
:   0-based index of the entity to remove

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRestraint::RemoveEntity.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

[ICWRestraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint_members.html)

[ICWRestraint::InsertEntity Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~InsertEntity.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0