<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetShellElementNormalAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetShellElementNormalAt Method (ICWMesh) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetShellElementNormalAt Method (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispFace*
:   Face

Gets shell normal for a face.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetShellElementNormalAt( _    ByVal DispFace As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim DispFace As System.Object Dim value As System.Integer   value = instance.GetShellElementNormalAt(DispFace) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetShellElementNormalAt(     System.object DispFace ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetShellElementNormalAt(  &   System.Object^ DispFace ) ``` | |

#### Parameters

*DispFace*
:   Face

#### Return Value

Shell normal for a face as defined at [swsMeshShellNormal\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshShellNormal_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::GetShellElementNormalAt.

# ![](dotnetimages/collapse.gif)Remarks

This method determines the positioning of the top and bottom faces of the shell elements associated with the face. The top face is towards the positive normal direction by default.

Use this method to align shells. [Flipping](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWMesh~FlipShellElements.html) switches the faces.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

[ICWMesh::UseJacobianCheckForShells Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~UseJacobianCheckForShells.html)

[ICWShell Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell.html)

[ICWShellManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP!.0