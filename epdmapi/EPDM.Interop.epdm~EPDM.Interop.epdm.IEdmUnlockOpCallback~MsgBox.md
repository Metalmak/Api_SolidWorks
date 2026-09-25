<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~MsgBox.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| MsgBox Method (IEdmUnlockOpCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUnlockOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html) : MsgBox Method (IEdmUnlockOpCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eMsg*
:   Message to display as defined in [EdmUnlockOpMsg](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockOpMsg.html)

*lDocID*
:   ID of the file that caused the message

*lProjID*
:   ID of the file's parent folder

*bsPath*
:   Full path to the file that caused the message

*poError*
:   [EdmUnlockErrInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockErrInfo.html) structure containing extended information about the error

Called by the check-in operation to display a message box with information or options that the user can choose.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function MsgBox( _    ByVal eMsg As EdmUnlockOpMsg, _    ByVal lDocID As System.Integer, _    ByVal lProjID As System.Integer, _    ByVal bsPath As System.String, _    ByRef poError As EdmUnlockErrInfo _ ) As EdmUnlockOpReply ``` | |

| C# |  |
| --- | --- |
| ``` EdmUnlockOpReply MsgBox(     EdmUnlockOpMsg eMsg,    System.int lDocID,    System.int lProjID,    System.string bsPath,    ref EdmUnlockErrInfo poError ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmUnlockOpReply MsgBox(  &   EdmUnlockOpMsg eMsg, &   System.int lDocID, &   System.int lProjID, &   System.String^ bsPath, &   EdmUnlockErrInfo% poError ) ``` | |

#### Parameters

*eMsg*
:   Message to display as defined in [EdmUnlockOpMsg](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockOpMsg.html)

*lDocID*
:   ID of the file that caused the message

*lProjID*
:   ID of the file's parent folder

*bsPath*
:   Full path to the file that caused the message

*poError*
:   [EdmUnlockErrInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockErrInfo.html) structure containing extended information about the error

#### Return Value

Reply to SOLIDWORKS PDM Professional as defined in [EdmUnlockOpReply](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockOpReply.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUnlockOpCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUnlockOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html)

[IEdmUnlockOpCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3