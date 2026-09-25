<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5~SendMsg.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SendMsg Method (IEdmUserGroup5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserGroup5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5.html) : SendMsg Method (IEdmUserGroup5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsSubject*
:   Email subject

*bsMessageText*
:   Message detail (see **Remarks**)

*bExcludeCurrentUser*
:   True to not send email to the logged-in user even if he is a member of this group, false to send email to the logged-in user

Sends email to all members of this user group.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SendMsg( _    ByVal bsSubject As System.String, _    ByVal bsMessageText As System.String, _    ByVal bExcludeCurrentUser As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SendMsg(     System.string bsSubject,    System.string bsMessageText,    System.bool bExcludeCurrentUser ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SendMsg(  &   System.String^ bsSubject, &   System.String^ bsMessageText, &   System.bool bExcludeCurrentUser ) ``` | |

#### Parameters

*bsSubject*
:   Email subject

*bsMessageText*
:   Message detail (see **Remarks**)

*bExcludeCurrentUser*
:   True to not send email to the logged-in user even if he is a member of this group, false to send email to the logged-in user

# ![](dotnetimages/collapse.gif)Example

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

It is possible to send HTML-formatted mail, if the recipients use a mail system that supports HTML. In so, add HTML tags to the text in bsMessageText:

> <html><body><h1>Hello!</h1>How are you?</body></html>

Call [IEdmUser5::SendMsg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5~SendMsg.html) to send email to an individual user.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserGroup5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5.html)

[IEdmUserGroup5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional version 5.2