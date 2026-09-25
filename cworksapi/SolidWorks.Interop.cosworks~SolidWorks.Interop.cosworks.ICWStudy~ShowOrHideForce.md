<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~ShowOrHideForce.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ShowOrHideForce Property (ICWStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : ShowOrHideForce Property (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Shows or hides the force symbols in the graphics area.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` WriteOnly Property ShowOrHideForce As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy   instance.ShowOrHideForce = value ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ShowOrHideForce {set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool ShowOrHideForce {    void set ( &   System.bool value); } ``` | |

#### Property Value

True to show force symbols in the study, false to hide them

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::ShowOrHideForces.

# ![](dotnetimages/collapse.gif)Example

[Analyze Part (C#)](Analyze_Part_Example_CSharp.htm)

[Analyze Part (VB.NET)](Analyze_Part_Example_VBNET.htm)

[Analyze Part (VBA)](Analyze_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::ShowOrHideFixtures Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~ShowOrHideFixtures.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2014 SP0