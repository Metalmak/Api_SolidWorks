<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5~SendMsg.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SendMsg Method (IEdmInbox5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmInbox5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5.html) : SendMsg Method (IEdmInbox5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsSubject*
:   Subject of the email

*bsMessageText*
:   Message detail (see **Remarks**)

Emails the current user.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SendMsg( _    ByVal bsSubject As System.String, _    ByVal bsMessageText As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SendMsg(     System.string bsSubject,    System.string bsMessageText ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SendMsg(  &   System.String^ bsSubject, &   System.String^ bsMessageText ) ``` | |

#### Parameters

*bsSubject*
:   Subject of the email

*bsMessageText*
:   Message detail (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUser5::SendMsg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5~SendMsg.html) example.

# ![](dotnetimages/collapse.gif)Remarks

It is possible to send HTML-formatted email, if the recipient uses a mail system that supports HTML. If so, then add HTML tags to the text in bsMessageText.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmInbox5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5.html)

[IEdmInbox5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5_members.html)

[IEdmUserGroup5::SendMsg Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5~SendMsg.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.3