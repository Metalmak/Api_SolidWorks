<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5~SendMsg.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SendMsg Method (IEdmUser5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUser5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5.html) : SendMsg Method (IEdmUser5) |

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

Sends email to this user.

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

[Send Message to Users (C#)](Send_Message_to_Users_Example_CSharp.htm)

[Send Message to Users (VB.NET)](Send_Message_to_Users_Example_VBNET.htm)

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

It is possible to send HTML-formatted mail, if the recipient uses a mail system that supports HTML. In so, add HTML tags to the text in bsMessageText.

For example, bsMessageText might contain:

> <html><body><h1>Hello!</h1>How are you?</body></html>

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUser5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5.html)

[IEdmUser5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5_members.html)

[IEdmUserGroup5::SendMsg Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5~SendMsg.html)

[IEdmInbox5::SendMsg Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5~SendMsg.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2