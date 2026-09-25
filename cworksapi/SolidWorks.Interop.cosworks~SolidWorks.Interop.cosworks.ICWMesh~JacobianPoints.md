<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~JacobianPoints.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| JacobianPoints Property (ICWMesh) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : JacobianPoints Property (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the number of points to be used in calculating a Jacobian ratio.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property JacobianPoints As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim value As System.Integer   instance.JacobianPoints = value   value = instance.JacobianPoints ``` | |

| C# |  |
| --- | --- |
| ``` System.int JacobianPoints {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int JacobianPoints {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Number of Jacobian points (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::JacobianPoints.

# ![](dotnetimages/collapse.gif)Remarks

This property:

* is valid only if [ICWMesh::Quality](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~Quality.html) is set to [swsMeshQuality\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshQuality_e.html).swsMeshQualityHigh.* has 4 possible values:
    + 4  = Number of points inside the element tetrahedron near its vertices+ 16 = Number of points inside the element tetrahedron+ 29 = Number of points inside the element tetrahedron (same as 16 but calculates a more precise Jacobian ratio)+ 10 = At nodes;  Number of points = 4 vertices + 6 midpoints on 6 edges of the element tetrahedron

For more information, read:

* The **Advanced** section of **Simulation > Meshing > Mesh PropertyManager** topic

    - and -

* The **Jacobian Points** section of the **Simulation > Meshing >** **Mesh Quality Checks** topic

in the SOLIDWORKS help.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

[ICWMesh::GetWorstJacobianRatio Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetWorstJacobianRatio.html)

[ICWMesh::NegativeJacobianRatioCheck Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~NegativeJacobianRatioCheck.html)

[ICWMesh::UseJacobianCheckForShells Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~UseJacobianCheckForShells.html)

[ICWMesh::UseJacobianCheckForSolids Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~UseJacobianCheckForSolids.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP0