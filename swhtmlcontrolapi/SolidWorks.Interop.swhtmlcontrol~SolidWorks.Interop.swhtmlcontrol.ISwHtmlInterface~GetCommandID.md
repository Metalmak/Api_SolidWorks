<!-- source: swhtmlcontrolapi/SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~GetCommandID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS HTML Control Type Library | Send comments on this topic. |
| GetCommandID Method (ISwHtmlInterface) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swhtmlcontrol Namespace](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol_namespace.html) > [ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html) : GetCommandID Method (ISwHtmlInterface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ClsID*
:   Add-in's class ID

*UserCmdID*
:   Unique ID that the add-in application identified as a CommandManager-style toolbar button

Gets the SOLIDWORKS resource ID for an add-in's CommandManager-style toolbar button.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCommandID( _    ByVal ClsID As System.String, _    ByVal UserCmdID As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwHtmlInterface Dim ClsID As System.String Dim UserCmdID As System.Integer Dim value As System.Integer   value = instance.GetCommandID(ClsID, UserCmdID) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetCommandID(     System.string ClsID,    System.int UserCmdID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetCommandID(  &   System.String^ ClsID, &   System.int UserCmdID ) ``` | |

#### Parameters

*ClsID*
:   Add-in's class ID

*UserCmdID*
:   Unique ID that the add-in application identified as a CommandManager-style toolbar button

#### Return Value

Currently bound ID for the CommandManager-style toolbar button

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwHtmlInterface::GetCommandID.

# ![](dotnetimages/collapse.gif)Example

[Flash an Add-in's Toolbar Button (VBA)](Flash_an_Add-in_s_Toolbar_Button_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html)

[ISwHtmlInterface Members](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface_members.html)

ISldWorks::ShowBubbleToolTip

[ISwHtmlInterface::ShowBubbleTooltip Method](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~ShowBubbleTooltip.html)

[ISwHtmlInterface::ShowBubbleTooltipForAddinToolbar Method](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~ShowBubbleTooltipForAddinToolbar.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 SP3, Revision Number 14.3