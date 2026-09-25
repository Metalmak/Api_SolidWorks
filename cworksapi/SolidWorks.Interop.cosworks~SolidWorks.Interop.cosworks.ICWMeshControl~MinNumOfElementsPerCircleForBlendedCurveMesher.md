<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~MinNumOfElementsPerCircleForBlendedCurveMesher.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| MinNumOfElementsPerCircleForBlendedCurveMesher Property (ICWMeshControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html) : MinNumOfElementsPerCircleForBlendedCurveMesher Property (ICWMeshControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the minimum number of elements in a circle to determine the maximum angle in a curvature-based mesh.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property MinNumOfElementsPerCircleForBlendedCurveMesher As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMeshControl Dim value As System.Integer   instance.MinNumOfElementsPerCircleForBlendedCurveMesher = value   value = instance.MinNumOfElementsPerCircleForBlendedCurveMesher ``` | |

| C# |  |
| --- | --- |
| ``` System.int MinNumOfElementsPerCircleForBlendedCurveMesher {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int MinNumOfElementsPerCircleForBlendedCurveMesher {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Minimum number of elements in a circle

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMeshControl::MinNumOfElementsPerCircleForBlendedCurveMesher.

# ![](dotnetimages/collapse.gif)Example

See the [ICWMeshControl](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if:

* [ICWMeshControl::BeamSelected](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~BeamSelected.html) = 0* [ICWMesh::MesherType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MesherType.html)=
    + [swsMesherType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMesherType_e.html).swsMesherTypeAlternateCB

     - or -

* swsMesherType\_e.swsMesherTypeAlternate

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html)

[ICWMeshControl Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl_members.html)

[ICWMeshControl::ElementSize Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~ElementSize.html)

[ICWMeshControl::Ratio Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~Ratio.html)

[ICWMeshControl::MinimumElementSizeForBlendedCurveMesher Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~MinimumElementSizeForBlendedCurveMesher.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0