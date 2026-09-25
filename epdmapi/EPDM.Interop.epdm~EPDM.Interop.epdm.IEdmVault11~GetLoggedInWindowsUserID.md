<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetLoggedInWindowsUserID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetLoggedInWindowsUserID Method (IEdmVault11) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html) : GetLoggedInWindowsUserID Method (IEdmVault11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsVault*
:   Name of the vault for which to get the logged-in user

Gets the ID of the user who is currently logged in through the SOLIDWORKS PDM Professional client software on this machine.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetLoggedInWindowsUserID( _    ByVal bsVault As System.String _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetLoggedInWindowsUserID(     System.string bsVault ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetLoggedInWindowsUserID(  &   System.String^ bsVault ) ``` | |

#### Parameters

*bsVault*
:   Name of the vault for which to get the logged-in user

#### Return Value

ID of the logged-in user; 0 if no one is logged in

# ![](dotnetimages/collapse.gif)Remarks

Any number of users can be logged into a vault at the same time by calling [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html). However, only a single user can be logged into a machine either through the SOLIDWORKS PDM Professional client software or by calling [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html). This is the user for whom this method returns an ID.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html)

[IEdmVault11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010