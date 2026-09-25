<!-- source: swhtmlcontrolapi/SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~ShowBubbleTooltipAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS HTML Control Type Library | Send comments on this topic. |
| ShowBubbleTooltipAt Method (ISwHtmlInterface) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swhtmlcontrol Namespace](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol_namespace.html) > [ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html) : ShowBubbleTooltipAt Method (ISwHtmlInterface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pointX*
:   x coordinate in pixels relative to upper-left corner of  screen

*pointY*
:   y coordinate in pixels relative to upper-left corner of screen

*arrowPos*
:   Arrow position as defined in swArrowPosition\_e

*titleString*
:   Title of Bubble ToolTip

*messageString*
:   Message string of Bubble ToolTip

*urlLoc*
:   Any valid Windows Internet Explorer file

Displays a Bubble ToolTip at the specified location.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowBubbleTooltipAt( _    ByVal pointX As System.Integer, _    ByVal pointY As System.Integer, _    ByVal arrowPos As System.Integer, _    ByVal titleString As System.String, _    ByVal messageString As System.String, _    ByVal urlLoc As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwHtmlInterface Dim pointX As System.Integer Dim pointY As System.Integer Dim arrowPos As System.Integer Dim titleString As System.String Dim messageString As System.String Dim urlLoc As System.String   instance.ShowBubbleTooltipAt(pointX, pointY, arrowPos, titleString, messageString, urlLoc) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowBubbleTooltipAt(     System.int pointX,    System.int pointY,    System.int arrowPos,    System.string titleString,    System.string messageString,    System.string urlLoc ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowBubbleTooltipAt(  &   System.int pointX, &   System.int pointY, &   System.int arrowPos, &   System.String^ titleString, &   System.String^ messageString, &   System.String^ urlLoc ) ``` | |

#### Parameters

*pointX*
:   x coordinate in pixels relative to upper-left corner of  screen

*pointY*
:   y coordinate in pixels relative to upper-left corner of screen

*arrowPos*
:   Arrow position as defined in swArrowPosition\_e

*titleString*
:   Title of Bubble ToolTip

*messageString*
:   Message string of Bubble ToolTip

*urlLoc*
:   Any valid Windows Internet Explorer file

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwHtmlInterface::ShowBubbleTooltipAt.

# ![](dotnetimages/collapse.gif)Example

**Visual Basic for Applications (VBA)**

This example shows how to display and hide a Bubble ToolTip.

'--------------------------------------------

'

' Preconditions: Substitute the path and filename of your HTML file for "*path\_filename*".

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

# ![](dotnetimages/collapse.gif)Example

[Show Bubble ToolTip (VBA)](Show_Bubble_ToolTip_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Remarks

|  |  |
| --- | --- |
| **If you specified a ...** | **Then the ToolTip's bubble...** |
| gif, .jpg, or .jpeg image for urlLoc | Is automatically expanded to accommodate the image |
| URL for urlLoc | Cannot be resized and shows only the URL |

# ![](dotnetimages/collapse.gif)See Also

####

[ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html)

[ISwHtmlInterface Members](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface_members.html)

[ISwHtmlInterface::ShowTooltip Method](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~ShowTooltip.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0