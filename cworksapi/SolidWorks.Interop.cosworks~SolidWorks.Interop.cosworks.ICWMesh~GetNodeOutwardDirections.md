<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetNodeOutwardDirections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetNodeOutwardDirections Method (ICWMesh) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetNodeOutwardDirections Method (ICWMesh) |

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

Gets the normal directions at all of the nodes on the surface of this mesh.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNodeOutwardDirections( _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetNodeOutwardDirections(ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetNodeOutwardDirections(     out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetNodeOutwardDirections(  &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*ErrorCode*
:   Error code as defined in [swsMeshQueryErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshQueryErrorCode_e.html)

#### Return Value

Array of x, y, and z coordinates of normal directions at all of the nodes on the surface of this mesh (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::GetNodeOutwardDirections.

# ![](dotnetimages/collapse.gif)Example

[Create Curvature-based Mesh (VBA)](Create_Curvature-based_Mesh_Example_VB.htm)

[Create Curvature-based Mesh (VB.NET)](Create_Curvature-based_Mesh_Example_VBNET.htm)

[Create Curvature-based Mesh (C#)](Create_Curvature-based_Mesh_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Array:

[

     x1, y1, z1,

     x2, y2, z2,

     ...,

     x*i*, y*i*, z*i*

]

where:

* x*i*, y*i*, z*i* is the normal direction at the *i*th node

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0