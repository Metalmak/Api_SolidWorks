<!-- source: swhtmlcontrolapi/SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~HideBubbleTooltip.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS HTML Control Type Library | Send comments on this topic. |
| HideBubbleTooltip Method (ISwHtmlInterface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swhtmlcontrol Namespace](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol_namespace.html) > [ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html) : HideBubbleTooltip Method (ISwHtmlInterface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Hides the Bubble ToolTip displayed by [ISwHtmlInterface::ShowBubbleTooltipAt](SOLIDWORKS.Interop.swhtmlcontrol~SOLIDWORKS.Interop.swhtmlcontrol.ISwHtmlInterface~ShowBubbleTooltipAt.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub HideBubbleTooltip() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwHtmlInterface   instance.HideBubbleTooltip() ``` | |

| C# |  |
| --- | --- |
| ``` void HideBubbleTooltip() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void HideBubbleTooltip(); ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwHtmlInterface::HideBubbleTooltip.

# ![](dotnetimages/collapse.gif)Example

**Visual Basic for Applications (VBA)**

This example shows how to display and hide a Bubble ToolTip.

'--------------------------------------------

'

' Preconditions: Substitute the path and filename of your HTML file for *path\_filename*.

'

' Postconditions: Contents of the HTML file are displayed in a Bubble ToolTip,

'                 and then are hidden from view.

'

'--------------------------------------------

Option Explicit

Sub main()

    Const sURLpath As String = "*path\_filename*"

    Dim pSldWorks As Object

    Set pSldWorks = CreateObject("SwHtmlControl.SwHtmlInterface")

    ' Show Bubble ToolTip

    pSldWorks.**ShowBubbleTooltipAt** 300, 400, swArrowLeftTop, "Sample Bubble ToolTip", "Message of Sample Bubble ToolTip", sURLpath

    Stop

    ' Hide Bubble ToolTip

    pSldWorks.**HidebubbleTooltip**

End Sub

'--------------------------------------------

# ![](dotnetimages/collapse.gif)See Also

####

[ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html)

[ISwHtmlInterface Members](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0