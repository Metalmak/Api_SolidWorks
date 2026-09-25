<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~NumofElementsforBeams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| NumofElementsforBeams Property (ICWMeshControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html) : NumofElementsforBeams Property (ICWMeshControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the total number of mesh elements for selected beams.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property NumofElementsforBeams As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMeshControl Dim value As System.Integer   instance.NumofElementsforBeams = value   value = instance.NumofElementsforBeams ``` | |

| C# |  |
| --- | --- |
| ``` System.int NumofElementsforBeams {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int NumofElementsforBeams {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Number of mesh elements for selected beams

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMeshControl::NumofElementsforBeams.

# ![](dotnetimages/collapse.gif)Example

See the [ICWMeshControl](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only for beams.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html)

[ICWMeshControl Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl_members.html)

[ICWMeshControl::ElementSize Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~ElementSize.html)

[ICWMeshControl::UseSameElementSize Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~UseSameElementSize.html)

[ICWMeshControl::BeamSelected Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~BeamSelected.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2011 SP0