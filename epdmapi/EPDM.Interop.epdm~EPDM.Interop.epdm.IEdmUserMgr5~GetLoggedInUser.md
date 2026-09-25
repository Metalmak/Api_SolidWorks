<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5~GetLoggedInUser.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetLoggedInUser Method (IEdmUserMgr5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html) : GetLoggedInUser Method (IEdmUserMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the user currently running this program in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetLoggedInUser() As IEdmUser5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmUser5 GetLoggedInUser() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmUser5^ GetLoggedInUser(); ``` | |

#### Return Value

[IEdmUser5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5.html); current user

# ![](dotnetimages/collapse.gif)Example

[Get Messages (C#)](Get_Messages_Example_CSharp.htm)

[Get Messages (VB.NET)](Get_Messages_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method returns the IEdmUser5 interface of the user currently logged in on the [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) object from which this IEdmUserMgr5 interface is retrieved. [IEdmUserMgr5::GetFirstLoggedInUserPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5~GetFirstLoggedInUserPosition.html) and [IEdmUserMgr5::GetNextLoggedInUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5~GetNextLoggedInUser.html) return information about all users currently logged in to the vault.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_NOT\_LOGGED\_IN: Neither [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) nor [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html) has been called.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html)

[IEdmUserMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2