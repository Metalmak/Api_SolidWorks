<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~ComputeFromMaterialDamping.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ComputeFromMaterialDamping Property (ICWDampingOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDampingOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html) : ComputeFromMaterialDamping Property (ICWDampingOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [ICWDampingOptions::ComputeFromMaterialDamping2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~ComputeFromMaterialDamping2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ComputeFromMaterialDamping As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDampingOptions Dim value As System.Integer   instance.ComputeFromMaterialDamping = value   value = instance.ComputeFromMaterialDamping ``` | |

| C# |  |
| --- | --- |
| ``` System.int ComputeFromMaterialDamping {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ComputeFromMaterialDamping {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

0 to not use the material damping ratio; 1 to use the material damping ratio (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDampingOptions::ComputeFromMaterialDamping.

# ![](dotnetimages/collapse.gif)Remarks

For more information about modal damping, see the SOLIDWORKS Simulation Help.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDampingOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html)

[ICWDampingOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions_members.html)

[ICWDampingOptions::GetDampingRatios Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~GetDampingRatios.html)

[ICWDampingOptions::SetDampingRatios Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~SetDampingRatios.html)

[ICWDampingOptions::DampingType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~DampingType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0