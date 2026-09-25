<!-- source: swhtmlcontrolapi/SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~ShowBubbleTooltip.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS HTML Control Type Library | Send comments on this topic. |
| ShowBubbleTooltip Method (ISwHtmlInterface) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swhtmlcontrol Namespace](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol_namespace.html) > [ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html) : ShowBubbleTooltip Method (ISwHtmlInterface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pointAt*
:   Toolbar button ID to which to point

*flashButtonIDs*
:   Array of toolbar buttons

*titleResID*
:   Title resource ID of Bubble Tooltip or 0

*titleString*
:   Title of Bubble ToolTip

*messageString*
:   Message string of Bubble ToolTip

Displays a Bubble ToolTip and flashes the specified toolbar button.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowBubbleTooltip( _    ByVal pointAt As System.Integer, _    ByVal flashButtonIDs As System.String, _    ByVal titleResID As System.Integer, _    ByVal titleString As System.String, _    ByVal messageString As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwHtmlInterface Dim pointAt As System.Integer Dim flashButtonIDs As System.String Dim titleResID As System.Integer Dim titleString As System.String Dim messageString As System.String   instance.ShowBubbleTooltip(pointAt, flashButtonIDs, titleResID, titleString, messageString) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowBubbleTooltip(     System.int pointAt,    System.string flashButtonIDs,    System.int titleResID,    System.string titleString,    System.string messageString ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowBubbleTooltip(  &   System.int pointAt, &   System.String^ flashButtonIDs, &   System.int titleResID, &   System.String^ titleString, &   System.String^ messageString ) ``` | |

#### Parameters

*pointAt*
:   Toolbar button ID to which to point

*flashButtonIDs*
:   Array of toolbar buttons

*titleResID*
:   Title resource ID of Bubble Tooltip or 0

*titleString*
:   Title of Bubble ToolTip

*messageString*
:   Message string of Bubble ToolTip

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwHtmlInterface::ShowBubbleTooltip.

# ![](dotnetimages/collapse.gif)Example

[Flash an Add-in's Toolbar Button (VBA)](Flash_an_Add-in_s_Toolbar_Button_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html)

[ISwHtmlInterface Members](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 SP3, Revision Number 14.3