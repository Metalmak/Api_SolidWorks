<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| LoginAuto Method (IEdmVault5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : LoginAuto Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsVaultName*
:   Vault name

*hParentWnd*
:   Parent window handle; used when the login dialog box displays to ensure it remains visible

Logs in to the specified vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub LoginAuto( _    ByVal bsVaultName As System.String, _    ByVal hParentWnd As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void LoginAuto(     System.string bsVaultName,    System.int hParentWnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LoginAuto(  &   System.String^ bsVaultName, &   System.int hParentWnd ) ``` | |

#### Parameters

*bsVaultName*
:   Vault name

*hParentWnd*
:   Parent window handle; used when the login dialog box displays to ensure it remains visible

# ![](dotnetimages/collapse.gif)Example

See the [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method differs from [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) in that this method does not require the username and password. This method logs into the vault as the same user that is already logged into either the vault view through File Explorer or the vault through the SOLIDWORKS PDM Professional client software. This method allows you to share the license of the already logged-in user. If no user is already logged into the specified file vault, a login dialog box displays. Also unlike IEdmVault5::Login, this method properly consumes a license without first calling [IEdmVault13::LoginEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault13~LoginEx.html) to comply with the [SOLIDWORKS End User License Agreement (EULA)](http://www.solidworks.com/sw/eula.htm).

You can retrieve the ID of the SOLIDWORKS PDM Professional client user by calling [IEdmVault11::GetLoggedInWindowsUserID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetLoggedInWindowsUserID.html). You can also log in silently as the SOLIDWORKS PDM Professional client by calling [IEdmVault11::LogInWindowsUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~LogInWindowsUser.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_ALREADY\_LOGGED\_IN: You are already logged in to this vault.* E\_EDM\_CANT\_OPEN\_DATABASE: The database could not be opened (Maybe the vault name was incorrect?).* E\_EDM\_CANCELLED\_BY\_USER: The log-in dialog box displays, but the user clicked **Cancel** instead of logging in.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2