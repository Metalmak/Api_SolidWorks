<!-- source: swinspectionapi/SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings~Shape.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Inspection API Help | Send comments on this topic. |
| Shape Property (IBalloonSettings) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swinspectionAddIn Namespace](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn_namespace.html) > [IBalloonSettings Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings.html) : Shape Property (IBalloonSettings) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the balloon shape for regular characteristics.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Shape As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBalloonSettings Dim value As System.Integer   instance.Shape = value   value = instance.Shape ``` | |

| C# |  |
| --- | --- |
| ``` System.int Shape {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int Shape {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Balloon shape as defined by [swiBalloonSettingsShape\_e](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.swiBalloonSettingsShape_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BalloonSettings properties.

# ![](dotnetimages/collapse.gif)See Also

####

[IBalloonSettings Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings.html)

[IBalloonSettings Members](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Inspection API 2022 FCS