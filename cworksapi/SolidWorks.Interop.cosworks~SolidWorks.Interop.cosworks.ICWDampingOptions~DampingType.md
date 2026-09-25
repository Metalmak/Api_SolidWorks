<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~DampingType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DampingType Property (ICWDampingOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDampingOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html) : DampingType Property (ICWDampingOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the damping type.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property DampingType As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDampingOptions Dim value As System.Integer   instance.DampingType = value   value = instance.DampingType ``` | |

| C# |  |
| --- | --- |
| ``` System.int DampingType {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int DampingType {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Damping type as defined in [swsDampingType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDampingType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDampingOptions::DampingType.

# ![](dotnetimages/collapse.gif)Example

See the [ICWDampingOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

For more information about damping, see the SOLIDWORKS Simulation Help.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDampingOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html)

[ICWDampingOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions_members.html)

[ICWDampingOptions::GetDampingRatios Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~GetDampingRatios.html)

[ICWDampingOptions::SetDampingRatios Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~SetDampingRatios.html)

[ICWDampingOptions::GetRayleighDampingCoefficients Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~GetRayleighDampingCoefficients.html)

[ICWDampingOptions::SetRayleighDampingCoefficients Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~SetRayleighDampingCoefficients.html)

[ICWDampingOptions::ComputeFromMaterialDamping Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~ComputeFromMaterialDamping.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0