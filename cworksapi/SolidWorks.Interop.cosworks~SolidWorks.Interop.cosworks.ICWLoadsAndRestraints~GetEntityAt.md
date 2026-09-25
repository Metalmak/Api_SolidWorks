<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraints~GetEntityAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetEntityAt Method (ICWLoadsAndRestraints) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraints Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraints.html) : GetEntityAt Method (ICWLoadsAndRestraints) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIndex*
:   0-based index of entity

*NSelType*
:   Entity type as defined in swSelectType\_e

Gets the entity at the specified index in this load or restraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEntityAt( _    ByVal NIndex As System.Integer, _    ByRef NSelType As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraints Dim NIndex As System.Integer Dim NSelType As System.Integer Dim value As System.Object   value = instance.GetEntityAt(NIndex, NSelType) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetEntityAt(     System.int NIndex,    out System.int NSelType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetEntityAt(  &   System.int NIndex, &   [Out] System.int NSelType ) ``` | |

#### Parameters

*NIndex*
:   0-based index of entity

*NSelType*
:   Entity type as defined in swSelectType\_e

#### Return Value

Entity

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraints::GetEntityAt.

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWLoadsAndRestraints::EntityCount](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWLoadsAndRestraints~EntityCount.html) before calling this method to get a valid value for NIndex.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraints Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraints.html)

[ICWLoadsAndRestraints Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraints_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0