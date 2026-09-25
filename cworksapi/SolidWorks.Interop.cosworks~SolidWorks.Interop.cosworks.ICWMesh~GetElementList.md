<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetElementList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetElementList Method (ICWMesh) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetElementList Method (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NElementType*
:   Type of elements in VarElementIDs as defined in [swsSimulationElementTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSimulationElementTypes_e.html)

*VarElementIDs*
:   Array of IDs of elements of type NElementType

Gets the elements of the specified type.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetElementList( _    ByVal NElementType As System.Integer, _    ByRef VarElementIDs As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim NElementType As System.Integer Dim VarElementIDs As System.Object Dim value As System.Integer   value = instance.GetElementList(NElementType, VarElementIDs) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetElementList(     System.int NElementType,    out System.object VarElementIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetElementList(  &   System.int NElementType, &   [Out] System.Object^ VarElementIDs ) ``` | |

#### Parameters

*NElementType*
:   Type of elements in VarElementIDs as defined in [swsSimulationElementTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSimulationElementTypes_e.html)

*VarElementIDs*
:   Array of IDs of elements of type NElementType

#### Return Value

Number of elements in VarElementIDs

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::GetElementList.

# ![](dotnetimages/collapse.gif)Example

[Get Mesh Elements and Nodes (VBA)](Get_Mesh_Elements_and_Nodes_Example_VB.htm)

[Get Mesh Elements and Nodes (VB.NET)](Get_Mesh_Elements_and_Nodes_Example_VBNET.htm)

[Get Mesh Elements and Nodes (C#)](Get_Mesh_Elements_And_Nodes_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

You must set [ICWMesh::Quality](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~Quality.html) to [swsMeshQuality\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshQuality_e.html).swsMeshQualityHigh before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

[ICWMesh::GetNodeList Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetNodeList.html)

[ICWMesh::GetSolidElementList Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetSolidElementList.html)

[ICWMesh::GetSolidNodeList Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetSolidNodeList.html)

[ICWMesh::GetSurfaceNodesAndNormals Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetSurfaceNodesAndNormals.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP05