<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeFriction2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| IncludeFriction2 Property (ICWContactComponent) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactComponent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html) : IncludeFriction2 Property (ICWContactComponent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sets whether to specify a friction coefficient for this contact.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property IncludeFriction2 As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactComponent Dim value As System.Boolean   instance.IncludeFriction2 = value   value = instance.IncludeFriction2 ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IncludeFriction2 {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool IncludeFriction2 {    System.bool get();    void set ( &   System.bool value); } ``` | |

#### Property Value

-1 or true to include friction, 0 or false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactComponent::IncludeFriction2.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only in static and nonlinear studies where [ICWContactComponent::ContactComponentType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ContactComponentType.html) is set to [swsContactType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactType_e.html).swsContactTypeStaticNoPenetration.

To set this property, you can specify either the boolean or the integer.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactComponent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html)

[ICWContactComponent Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0