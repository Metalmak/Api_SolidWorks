<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ClearanceUnit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ClearanceUnit Property (ICWContactComponent) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactComponent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html) : ClearanceUnit Property (ICWContactComponent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the units of clearance between non-touching faces.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ClearanceUnit As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactComponent Dim value As System.Integer   instance.ClearanceUnit = value   value = instance.ClearanceUnit ``` | |

| C# |  |
| --- | --- |
| ``` System.int ClearanceUnit {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ClearanceUnit {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Units of clearance as defined in [swsPinballUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPinballUnit_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactComponent::ClearanceUnit.

# ![](dotnetimages/collapse.gif)Example

See the [ICWContactComponent](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

| This property is valid only if... | Is set to... |
| --- | --- |
| [ICWContactComponent::ContactComponentType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ContactComponentType.html) | [swsContactType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactType_e.html).swsContactTypeBonded |
| [ICWContactComponent::IncludeClearance](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeClearance.html) | 1 |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactComponent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html)

[ICWContactComponent Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent_members.html)

[ICWContactComponent::ClearanceValue Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ClearanceValue.html)

[ICWContactComponent::IncludeShellEdgeSolidOrShellFace Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeShellEdgeSolidOrShellFace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0