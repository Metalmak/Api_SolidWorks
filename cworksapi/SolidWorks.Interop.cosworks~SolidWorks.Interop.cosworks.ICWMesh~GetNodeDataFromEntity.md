<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetNodeDataFromEntity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetNodeDataFromEntity Method (ICWMesh) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetNodeDataFromEntity Method (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Entity

*NCount*
:   Number of nodes

Gets the node data associated with an entity.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNodeDataFromEntity( _    ByVal DispEntity As System.Object, _    ByRef NCount As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim DispEntity As System.Object Dim NCount As System.Integer Dim value As System.Object   value = instance.GetNodeDataFromEntity(DispEntity, NCount) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetNodeDataFromEntity(     System.object DispEntity,    out System.int NCount ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetNodeDataFromEntity(  &   System.Object^ DispEntity, &   [Out] System.int NCount ) ``` | |

#### Parameters

*DispEntity*
:   Entity

*NCount*
:   Number of nodes

#### Return Value

Array of nodal data (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::GetNodeDataFromEntity.

# ![](dotnetimages/collapse.gif)Remarks

Probe functionality.

Array of nodal data:

[

*N1, X1, Y1, Z1,*

*N2, X2, Y2, Z2,*

*...,*

*Ni,**Xi, Yi, Zi*

 ]

where:

* N*i* = *i*th node number

  * X*i*, Y*i*, Z*i* = coordinates of node N*i*

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

[ICWMesh::GetNodeLocation Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetNodeLocation.html)

[ICWMesh::GetNodes Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetNodes.html)

[ICWMesh::NodeCount Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~NodeCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0