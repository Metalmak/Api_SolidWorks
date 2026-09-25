<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetSurfaceNodesAndNormals.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetSurfaceNodesAndNormals Method (ICWMesh) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetSurfaceNodesAndNormals Method (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarNodeIDs*
:   Array of node IDs (see **Remarks**)

*VarNumNormals*
:   Array of numbers (1, 2 or 3) of normal vectors for the corresponding node ID in VarNodeIDs (see **Remarks**)

*VarNormalVecs*
:   Array of normal vectors (see **Remarks**)

Gets the nodes and normal vectors at the surface of this solid mesh.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSurfaceNodesAndNormals( _    ByRef VarNodeIDs As System.Object, _    ByRef VarNumNormals As System.Object, _    ByRef VarNormalVecs As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim VarNodeIDs As System.Object Dim VarNumNormals As System.Object Dim VarNormalVecs As System.Object Dim value As System.Integer   value = instance.GetSurfaceNodesAndNormals(VarNodeIDs, VarNumNormals, VarNormalVecs) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSurfaceNodesAndNormals(     out System.object VarNodeIDs,    out System.object VarNumNormals,    out System.object VarNormalVecs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSurfaceNodesAndNormals(  &   [Out] System.Object^ VarNodeIDs, &   [Out] System.Object^ VarNumNormals, &   [Out] System.Object^ VarNormalVecs ) ``` | |

#### Parameters

*VarNodeIDs*
:   Array of node IDs (see **Remarks**)

*VarNumNormals*
:   Array of numbers (1, 2 or 3) of normal vectors for the corresponding node ID in VarNodeIDs (see **Remarks**)

*VarNormalVecs*
:   Array of normal vectors (see **Remarks**)

#### Return Value

Number of nodes

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::GetSurfaceNodesAndNormals.

# ![](dotnetimages/collapse.gif)Example

[Get Mesh Elements and Nodes (VBA)](Get_Mesh_Elements_and_Nodes_Example_VB.htm)

[Get Mesh Elements and Nodes (VB.NET)](Get_Mesh_Elements_and_Nodes_Example_VBNET.htm)

[Get Mesh Elements and Nodes (C#)](Get_Mesh_Elements_And_Nodes_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

You must set [ICWMesh::Quality](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~Quality.html) to [swsMeshQuality\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshQuality_e.html).swsMeshQualityHigh before calling this method.

Each node can have one or more normal vectors. For example, for a meshed cube:

| Node location | Number of normal vectors |
| --- | --- |
| Middle of side | 1 |
| Edge | 2 |
| Vertex | 3 |

VarNormalVecs contains an array of all of the normal vectors:

[

*xa1, ya1, za1, xb1, yb1, zb1, xc1, yc1, zc1,*

*xa2, ya2, za2,*

*...,*

*xai, yai, zai*

]

where:

* *x*, *y*, and *z* denote location* *a*, *b*, and *c* denote normal vectors* *xai*, *yai*, *zai* denote the location of the *a*th normal vector for the *i*th node

Use VarNumNormals to calculate which vectors in VarNormalVecs map to the node IDs in VarNodeIDs.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

[ICWMesh::GetElementList Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetElementList.html)

[ICWMesh::GetNodeList Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetNodeList.html)

[ICWMesh::GetSolidElementList Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetSolidElementList.html)

[ICWMesh::GetSolidNodeList Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetSolidNodeList.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP05