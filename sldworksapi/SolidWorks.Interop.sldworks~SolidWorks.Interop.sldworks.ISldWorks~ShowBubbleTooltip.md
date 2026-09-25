<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ShowBubbleTooltip.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowBubbleTooltip Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : ShowBubbleTooltip Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PointAt*
:   Toolbar button ID

*FlashButtonIDs*
:   Array of strings for the toolbar buttons

*TitleResID*
:   Title resource ID of bubble Tooltip or 0

*TitleString*
:   Title of bubble ToolTip

*MessageString*
:   Message string of bubble ToolTip

Displays a bubble ToolTip and flashes the specified toolbar button.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowBubbleTooltip( _    ByVal PointAt As System.Integer, _    ByVal FlashButtonIDs As System.String, _    ByVal TitleResID As System.Integer, _    ByVal TitleString As System.String, _    ByVal MessageString As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim PointAt As System.Integer Dim FlashButtonIDs As System.String Dim TitleResID As System.Integer Dim TitleString As System.String Dim MessageString As System.String   instance.ShowBubbleTooltip(PointAt, FlashButtonIDs, TitleResID, TitleString, MessageString) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowBubbleTooltip(     System.int PointAt,    System.string FlashButtonIDs,    System.int TitleResID,    System.string TitleString,    System.string MessageString ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowBubbleTooltip(  &   System.int PointAt, &   System.String^ FlashButtonIDs, &   System.int TitleResID, &   System.String^ TitleString, &   System.String^ MessageString ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PointAt*
:   Toolbar button ID

*FlashButtonIDs*
:   Array of strings for the toolbar buttons

*TitleResID*
:   Title resource ID of bubble Tooltip or 0

*TitleString*
:   Title of bubble ToolTip

*MessageString*
:   Message string of bubble ToolTip

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::ShowBubbleTooltip.

# ![](dotnetimages/collapse.gif)Example

[Flash an Add-in's Toolbar Button (VBA)](Flash_an_Add-in_s_Toolbar_Button_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::ShowBubbleTooltipAt2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ShowBubbleTooltipAt2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 SP3, Revision Number 14.3