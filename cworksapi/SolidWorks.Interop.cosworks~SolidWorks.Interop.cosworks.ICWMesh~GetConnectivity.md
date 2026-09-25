<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetConnectivity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetConnectivity Method (ICWMesh) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetConnectivity Method (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ErrorCode*
:   Error code as defined in [swsMeshQueryErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshQueryErrorCode_e.html)

Gets the connectivity of nodes on the surface of the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetConnectivity( _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetConnectivity(ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetConnectivity(     out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetConnectivity(  &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*ErrorCode*
:   Error code as defined in [swsMeshQueryErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshQueryErrorCode_e.html)

#### Return Value

Array of node connectivity data (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::GetConnectivity.

# ![](dotnetimages/collapse.gif)Example

[Create Curvature-based Mesh (VBA)](Create_Curvature-based_Mesh_Example_VB.htm)

[Create Curvature-based Mesh (VB.NET)](Create_Curvature-based_Mesh_Example_VBNET.htm)

[Create Curvature-based Mesh (C#)](Create_Curvature-based_Mesh_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Array of node connectivity data:

[

     c1, n11, n12, n13,

     c2, n21, n22, n23,

     ...,

     c*i*, n*i*1, n*i*2, n*i*3

]

where:

* c*i* is number of nodes in the *i*th connectivity unit; 2 for beams, 3 for solids and shells, 4 for hexagons* n*i*1, n*i*2, n*i*3 are the nodes in the *i*th connectivity unit

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0