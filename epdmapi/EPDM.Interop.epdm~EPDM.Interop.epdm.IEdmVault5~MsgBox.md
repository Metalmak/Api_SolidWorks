<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~MsgBox.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| MsgBox Method (IEdmVault5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : MsgBox Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*bsMsg*
:   Message to display in the message box

*eType*
:   Optional style of the message box as defined in [EdmMBoxType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMBoxType.html)

*bsCaption*
:   Optional string to display for the message box caption

Displays a message box to the user.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function MsgBox( _    ByVal lParentWnd As System.Integer, _    ByVal bsMsg As System.String, _    Optional ByVal eType As EdmMBoxType, _    Optional ByVal bsCaption As System.String _ ) As EdmMBoxResult ``` | |

| C# |  |
| --- | --- |
| ``` EdmMBoxResult MsgBox(     System.int lParentWnd,    System.string bsMsg,    EdmMBoxType eType,    System.string bsCaption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmMBoxResult MsgBox(  &   System.int lParentWnd, &   System.String^ bsMsg, &   EdmMBoxType eType, &   System.String^ bsCaption ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*bsMsg*
:   Message to display in the message box

*eType*
:   Optional style of the message box as defined in [EdmMBoxType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMBoxType.html)

*bsCaption*
:   Optional string to display for the message box caption

#### Return Value

Button clicked as defined in [EdmMBoxResult](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMBoxResult.html)

# ![](dotnetimages/collapse.gif)Example

[Notify User When File Changes State (VB.NET)](Notify_User_When_File_Changes_State_Example_VBNET.htm)

[Notify User When File Changes State (C#)](Notify_User_When_File_Changes_State_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The only advantage of this method over the standard Visual Basic MsgBox function is that, with this method, you can specify a parent window handle to ensure that the message box stays on top of whatever parent window you have. For add-ins the parent window is usually the File Explorer window.

You do not need to call [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) or [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html) before calling this method.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The user pressed **Cancel**.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2