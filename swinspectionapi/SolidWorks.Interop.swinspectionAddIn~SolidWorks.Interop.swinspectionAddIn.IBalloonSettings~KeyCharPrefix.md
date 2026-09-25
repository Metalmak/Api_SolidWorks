<!-- source: swinspectionapi/SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings~KeyCharPrefix.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Inspection API Help | Send comments on this topic. |
| KeyCharPrefix Property (IBalloonSettings) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swinspectionAddIn Namespace](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn_namespace.html) > [IBalloonSettings Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings.html) : KeyCharPrefix Property (IBalloonSettings) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the prefix to add to the balloons for key characteristics.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property KeyCharPrefix As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBalloonSettings Dim value As System.String   instance.KeyCharPrefix = value   value = instance.KeyCharPrefix ``` | |

| C# |  |
| --- | --- |
| ``` System.string KeyCharPrefix {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ KeyCharPrefix {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

#### Property Value

Prefix

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BalloonSettings properties.

# ![](dotnetimages/collapse.gif)Remarks

Key characteristics are characteristics whose variation has a significant impact on the quality of the part.

# ![](dotnetimages/collapse.gif)See Also

####

[IBalloonSettings Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings.html)

[IBalloonSettings Members](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Inspection API 2022 FCS