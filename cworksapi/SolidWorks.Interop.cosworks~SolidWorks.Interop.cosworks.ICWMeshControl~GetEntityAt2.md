<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~GetEntityAt2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetEntityAt2 Method (ICWMeshControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html) : GetEntityAt2 Method (ICWMeshControl) |

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

*BExcludeVertexAndReference*
:   True to exclude the vertex and reference, false to not

*NSelectionType*
:   Type of entity as defined in swSelectType\_e

Obsolete. Superseded by [ICWMeshControl::GetEntityAt3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~GetEntityAt3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEntityAt2( _    ByVal NIndex As System.Integer, _    ByVal BExcludeVertexAndReference As System.Integer, _    ByRef NSelectionType As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMeshControl Dim NIndex As System.Integer Dim BExcludeVertexAndReference As System.Integer Dim NSelectionType As System.Integer Dim value As System.Object   value = instance.GetEntityAt2(NIndex, BExcludeVertexAndReference, NSelectionType) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetEntityAt2(     System.int NIndex,    System.int BExcludeVertexAndReference,    out System.int NSelectionType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetEntityAt2(  &   System.int NIndex, &   System.int BExcludeVertexAndReference, &   [Out] System.int NSelectionType ) ``` | |

#### Parameters

*NIndex*
:   0-based index of entity

*BExcludeVertexAndReference*
:   True to exclude the vertex and reference, false to not

*NSelectionType*
:   Type of entity as defined in swSelectType\_e

#### Return Value

Entity

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMeshControl::GetEntityAt2.

# ![](dotnetimages/collapse.gif)Remarks

To specify NIndex, use [ICWMeshControl::EntityCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~EntityCount.html) to determine the number of entities in this mesh control.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html)

[ICWMeshControl Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl_members.html)

[ICWMeshControl::InsertEntity Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~InsertEntity.html)

[ICWMeshControl::RemoveEntity Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~RemoveEntity.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP2