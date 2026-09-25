<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~CopyMeshFromStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CopyMeshFromStudy Method (ICWStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : CopyMeshFromStudy Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SStudyName*
:   Name of study from which to copy a mesh

Copies the mesh from the specified study to this study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CopyMeshFromStudy( _    ByVal SStudyName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim SStudyName As System.String Dim value As System.Integer   value = instance.CopyMeshFromStudy(SStudyName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CopyMeshFromStudy(     System.string SStudyName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CopyMeshFromStudy(  &   System.String^ SStudyName ) ``` | |

#### Parameters

*SStudyName*
:   Name of study from which to copy a mesh

#### Return Value

Error code as defined in [swsMeshCopyErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshCopyErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::CopyMeshFromStudy.

# ![](dotnetimages/collapse.gif)Example

[Copy Mesh and Generate Report (VBA)](Copy_Mesh_and_Gen_Report_Example_VB.htm)

[Copy Mesh and Generate Report (VB.NET)](Copy_Mesh_and_Gen_Report_Example_VBNET.htm)

[Copy Mesh and Generate Report (C#)](Copy_Mesh_and_Gen_Report_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::CreateMesh Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~CreateMesh.html)

[ICWStudy::Mesh Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~Mesh.html)

[ICWStudy::MeshType Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~MeshType.html)

[ICWStudy::MeshAndRun Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~MeshAndRun.html)

[ICWStudy::CreateMeshForMeshControl Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~CreateMeshForMeshControl.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0