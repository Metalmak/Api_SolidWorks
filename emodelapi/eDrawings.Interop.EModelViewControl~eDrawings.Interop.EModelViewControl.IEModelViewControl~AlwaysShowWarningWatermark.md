<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~AlwaysShowWarningWatermark.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| AlwaysShowWarningWatermark Property (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : AlwaysShowWarningWatermark Property (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to show a warning watermark when an existing file is opened.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AlwaysShowWarningWatermark As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim value As System.Integer   instance.AlwaysShowWarningWatermark = value   value = instance.AlwaysShowWarningWatermark ``` | |

| C# |  |
| --- | --- |
| ``` System.int AlwaysShowWarningWatermark {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int AlwaysShowWarningWatermark {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

-1 to show a warning watermark, 0 to not show a warning watermark

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::AlwaysShowWarningWatermark.

# ![](dotnetimages/collapse.gif)Remarks

eDrawings detects when the graphics data for a component might not be synchronized with a later version of the file that was modified and saved in a SOLIDWORKS assembly. When a potentially outdated component is opened, a watermark displays a warning and suggests that the part in the SOLIDWORKS software be rebuilt.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

[IEModelViewControl::OpenDoc Method](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~OpenDoc.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2012 SP0