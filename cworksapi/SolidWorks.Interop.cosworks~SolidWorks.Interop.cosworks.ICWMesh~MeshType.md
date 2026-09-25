<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MeshType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| MeshType Property (ICWMesh) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : MeshType Property (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Returns the mesh type.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property MeshType As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim value As System.Integer   value = instance.MeshType ``` | |

| C# |  |
| --- | --- |
| ``` System.int MeshType {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int MeshType {    System.int get(); } ``` | |

#### Property Value

Mesh type as defined in [swsMeshType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshType_e.html) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::MeshType.

# ![](dotnetimages/collapse.gif)Remarks

Valid mesh types for different types of studies:

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| Study Type | Solid Mesh | Shell Mesh | Mixed Mesh (Solid & Shell) | Beam Mesh |
| Static | Supported | Supported | Supported | Supported |
| Frequency | Supported | Supported | Supported | Supported |
| Buckling | Supported | Supported | Supported | Supported |
| Thermal | Supported | Supported | Supported | Supported |
| Nonlinear | Supported | Supported | Supported | Not Supported |
| Linear Dynamic | Supported | Supported | Supported | Not Supported |
| Drop Test | Supported | Not Supported | Not Supported | Not Supported |
| Fatigue | Not Applicable | Not Applicable | Not Applicable | Not Applicable |
| Optimization | Not Applicable | Not Applicable | Not Applicable | Not Applicable |

**NOTES:**

* For documents with surface geometry only (no solids), only RefSurfShellElementMesh is supported.

  * BeamElementMesh is supported only for static, buckling, and frequency studies.

    * Drop test studies support solid mesh only.

      * Optimization and fatigue studies do not have mesh on their own. They use mesh of referenced studies. Mesh type is set to SolidElementMesh.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0