<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDistributedMass~InsertEntity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| InsertEntity Method (ICWDistributedMass) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDistributedMass Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDistributedMass.html) : InsertEntity Method (ICWDistributedMass) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Face or edge

Adds a face or shell edge to the collection of entities on which to distribute the mass.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertEntity( _    ByVal DispEntity As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDistributedMass Dim DispEntity As System.Object Dim value As System.Integer   value = instance.InsertEntity(DispEntity) ``` | |

| C# |  |
| --- | --- |
| ``` System.int InsertEntity(     System.object DispEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int InsertEntity(  &   System.Object^ DispEntity ) ``` | |

#### Parameters

*DispEntity*
:   Face or edge

#### Return Value

Index of entity added

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDistributedMass::InsertEntity.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDistributedMass Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDistributedMass.html)

[ICWDistributedMass Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDistributedMass_members.html)

[ICWDistributedMass::RemoveEntity Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDistributedMass~RemoveEntity.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0