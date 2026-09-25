<!-- source: swhtmlcontrolapi/SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~ShowBubbleTooltipForAddinToolbar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS HTML Control Type Library | Send comments on this topic. |
| ShowBubbleTooltipForAddinToolbar Method (ISwHtmlInterface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swhtmlcontrol Namespace](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol_namespace.html) > [ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html) : ShowBubbleTooltipForAddinToolbar Method (ISwHtmlInterface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*addInCLSID*
:   Add-in's class ID

*pointAt\_UserID*
:   Toolbar button ID to which to point

*flashButton\_UserIDs*
:   Array of toolbar buttons

*titleResID*
:   Title resource ID of Bubble Tooltip or 0

*titleString*
:   Title of Bubble ToolTip

*messageString*
:   Message string of Bubble ToolTip

Displays a Bubble Tooltip for the specified add-in and flashes the specified toolbar button.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowBubbleTooltipForAddinToolbar( _    ByVal addInCLSID As System.String, _    ByVal pointAt_UserID As System.Integer, _    ByVal flashButton_UserIDs As System.String, _    ByVal titleResID As System.Integer, _    ByVal titleString As System.String, _    ByVal messageString As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwHtmlInterface Dim addInCLSID As System.String Dim pointAt_UserID As System.Integer Dim flashButton_UserIDs As System.String Dim titleResID As System.Integer Dim titleString As System.String Dim messageString As System.String   instance.ShowBubbleTooltipForAddinToolbar(addInCLSID, pointAt_UserID, flashButton_UserIDs, titleResID, titleString, messageString) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowBubbleTooltipForAddinToolbar(     System.string addInCLSID,    System.int pointAt_UserID,    System.string flashButton_UserIDs,    System.int titleResID,    System.string titleString,    System.string messageString ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowBubbleTooltipForAddinToolbar(  &   System.String^ addInCLSID, &   System.int pointAt_UserID, &   System.String^ flashButton_UserIDs, &   System.int titleResID, &   System.String^ titleString, &   System.String^ messageString ) ``` | |

#### Parameters

*addInCLSID*
:   Add-in's class ID

*pointAt\_UserID*
:   Toolbar button ID to which to point

*flashButton\_UserIDs*
:   Array of toolbar buttons

*titleResID*
:   Title resource ID of Bubble Tooltip or 0

*titleString*
:   Title of Bubble ToolTip

*messageString*
:   Message string of Bubble ToolTip

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwHtmlInterface::ShowBubbleTooltipForAddinToolbar.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html)

[ISwHtmlInterface Members](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface_members.html)

ISldWorks::ShowBubbleTooltip

[ISwHtmlInterface::GetCommandID Method](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~GetCommandID.html)

[ISwHtmlInterface::ShowBubbleTooltip Method](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~ShowBubbleTooltip.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0