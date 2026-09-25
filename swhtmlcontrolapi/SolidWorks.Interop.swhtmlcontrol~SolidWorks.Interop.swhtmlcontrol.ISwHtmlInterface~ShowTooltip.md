<!-- source: swhtmlcontrolapi/SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~ShowTooltip.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS HTML Control Type Library | Send comments on this topic. |
| ShowTooltip Method (ISwHtmlInterface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swhtmlcontrol Namespace](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol_namespace.html) > [ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html) : ShowTooltip Method (ISwHtmlInterface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ToolbarName*
:   Name of toolbar

*buttonIndex*
:   0-based index indicating a toolbar button

*mask1*
:   0-31 bitmask indicating the toolbar buttons to flash

*mask2*
:   32-63 bitmask indicating the toolbar buttons to flash

*titleString*
:   Title of Bubble ToolTip

*messageString*
:   Message of Bubble ToolTip

Shows the Bubble ToolTip and flashes the specified toolbar or toolbar buttons.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowTooltip( _    ByVal ToolbarName As System.String, _    ByVal buttonIndex As System.Integer, _    ByVal mask1 As System.Integer, _    ByVal mask2 As System.Integer, _    ByVal titleString As System.String, _    ByVal messageString As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwHtmlInterface Dim ToolbarName As System.String Dim buttonIndex As System.Integer Dim mask1 As System.Integer Dim mask2 As System.Integer Dim titleString As System.String Dim messageString As System.String   instance.ShowTooltip(ToolbarName, buttonIndex, mask1, mask2, titleString, messageString) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowTooltip(     System.string ToolbarName,    System.int buttonIndex,    System.int mask1,    System.int mask2,    System.string titleString,    System.string messageString ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowTooltip(  &   System.String^ ToolbarName, &   System.int buttonIndex, &   System.int mask1, &   System.int mask2, &   System.String^ titleString, &   System.String^ messageString ) ``` | |

#### Parameters

*ToolbarName*
:   Name of toolbar

*buttonIndex*
:   0-based index indicating a toolbar button

*mask1*
:   0-31 bitmask indicating the toolbar buttons to flash

*mask2*
:   32-63 bitmask indicating the toolbar buttons to flash

*titleString*
:   Title of Bubble ToolTip

*messageString*
:   Message of Bubble ToolTip

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwHtmlInterface::ShowTooltip.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html)

[ISwHtmlInterface Members](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0