<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6~MsgBox.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| MsgBox Method (IEdmCallback6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) : MsgBox Method (IEdmCallback6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Handle of the parent window

*lMsgID*
:   ID of the message to be shown (see **Remarks**)

*bsMsg*
:   Message to be displayed

*eType*
:   Message box type as defined in [EdmMBoxType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMBoxType.html)

Displays a message box.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function MsgBox( _    ByVal lParentWnd As System.Integer, _    ByVal lMsgID As System.Integer, _    ByVal bsMsg As System.String, _    Optional ByVal eType As EdmMBoxType _ ) As EdmMBoxResult ``` | |

| C# |  |
| --- | --- |
| ``` EdmMBoxResult MsgBox(     System.int lParentWnd,    System.int lMsgID,    System.string bsMsg,    EdmMBoxType eType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmMBoxResult MsgBox(  &   System.int lParentWnd, &   System.int lMsgID, &   System.String^ bsMsg, &   EdmMBoxType eType ) ``` | |

#### Parameters

*lParentWnd*
:   Handle of the parent window

*lMsgID*
:   ID of the message to be shown (see **Remarks**)

*bsMsg*
:   Message to be displayed

*eType*
:   Message box type as defined in [EdmMBoxType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMBoxType.html)

#### Return Value

Message box result as defined in [EdmMBoxResult](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMBoxResult.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

For callbacks during add operations, IMsgID is one of the values defined in [EdmAddCallbackMsgID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddCallbackMsgID.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* <any error code>: The calling method terminated.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html)

[IEdmCallback6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0