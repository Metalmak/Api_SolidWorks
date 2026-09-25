<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~PoissonsRatio.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| PoissonsRatio Property (ICWLinkageRod) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLinkageRod Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html) : PoissonsRatio Property (ICWLinkageRod) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sets the Poisson's Ratio for the custom material of this linkage rod connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` WriteOnly Property PoissonsRatio As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLinkageRod   instance.PoissonsRatio = value ``` | |

| C# |  |
| --- | --- |
| ``` System.double PoissonsRatio {set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double PoissonsRatio {    void set ( &   System.double value); } ``` | |

#### Property Value

0.0 <= Poisson's Ratio <= 1.0

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLinkageRod::PoissonsRatio.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ICWLinkageRod::MaterialSource](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~MaterialSource.html) is set to [swsMaterialSourceType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMaterialSourceType_e.html).swsMaterial\_Custom.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLinkageRod Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html)

[ICWLinkageRod Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0