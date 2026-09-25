<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~GetEntityAt3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetEntityAt3 Method (ICWMeshControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html) : GetEntityAt3 Method (ICWMeshControl) |

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
:   -1 or true to exclude the vertex and reference, 0 or false to not

*NSelectionType*
:   Type of entity as defined in swSelectType\_e

Gets the entity at the specified index for this mesh control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEntityAt3( _    ByVal NIndex As System.Integer, _    ByVal BExcludeVertexAndReference As System.Boolean, _    ByRef NSelectionType As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMeshControl Dim NIndex As System.Integer Dim BExcludeVertexAndReference As System.Boolean Dim NSelectionType As System.Integer Dim value As System.Object   value = instance.GetEntityAt3(NIndex, BExcludeVertexAndReference, NSelectionType) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetEntityAt3(     System.int NIndex,    System.bool BExcludeVertexAndReference,    out System.int NSelectionType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetEntityAt3(  &   System.int NIndex, &   System.bool BExcludeVertexAndReference, &   [Out] System.int NSelectionType ) ``` | |

#### Parameters

*NIndex*
:   0-based index of entity

*BExcludeVertexAndReference*
:   -1 or true to exclude the vertex and reference, 0 or false to not

*NSelectionType*
:   Type of entity as defined in swSelectType\_e

#### Return Value

Entity

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html)

[ICWMeshControl Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30