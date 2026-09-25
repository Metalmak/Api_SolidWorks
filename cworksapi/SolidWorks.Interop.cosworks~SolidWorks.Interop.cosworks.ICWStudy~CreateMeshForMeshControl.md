<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~CreateMeshForMeshControl.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateMeshForMeshControl Method (ICWStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : CreateMeshForMeshControl Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SMeshControlName*
:   Name of the mesh control

Creates a mesh for the specified mesh control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateMeshForMeshControl( _    ByVal SMeshControlName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim SMeshControlName As System.String Dim value As System.Integer   value = instance.CreateMeshForMeshControl(SMeshControlName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreateMeshForMeshControl(     System.string SMeshControlName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreateMeshForMeshControl(  &   System.String^ SMeshControlName ) ``` | |

#### Parameters

*SMeshControlName*
:   Name of the mesh control

#### Return Value

Error as defined in [swsMeshControlMeshingError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshControlMeshingError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::CreateMeshForMeshControl.

# ![](dotnetimages/collapse.gif)Example

[Apply Mesh Control (VBA)](Apply_Mesh_Control_Example_VB.htm)

[Apply Mesh Control (VB.NET)](Apply_Mesh_Control_Example_VBNET.htm)

[Apply Mesh Control (C#)](Apply_Mesh_Control_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To populate SMeshControlName, call:

1. [ICWMesh::GetMeshControlAt](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetMeshControlAt.html)- [ICWMeshControl::Name](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~Name.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::CreateMesh Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~CreateMesh.html)

[ICWStudy::MeshAndRun Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~MeshAndRun.html)

[ICWStudy::CopyMeshFromStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~CopyMeshFromStudy.html)

[ICWStudy::Mesh Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~Mesh.html)

[ICWStudy::MeshType Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~MeshType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0