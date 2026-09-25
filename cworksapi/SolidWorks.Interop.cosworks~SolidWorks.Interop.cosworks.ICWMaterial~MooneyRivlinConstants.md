<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~MooneyRivlinConstants.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| MooneyRivlinConstants Property (ICWMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : MooneyRivlinConstants Property (ICWMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the Mooney Rivlin constants for the MooneyRivlin material
model used in nonlinear studies only.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property MooneyRivlinConstants As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim value As System.Integer   instance.MooneyRivlinConstants = value   value = instance.MooneyRivlinConstants ``` | |

| C# |  |
| --- | --- |
| ``` System.int MooneyRivlinConstants {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int MooneyRivlinConstants {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Number of Mooney Rivlin constants

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMaterial::MooneyRivlinConstants.

# ![](dotnetimages/collapse.gif)Remarks

Mooney Rivlin constants are valid in nonlinear studies only.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0