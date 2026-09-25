<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Login Method (IEdmVault5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : Login Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsUserName*
:   User name of user created in the SOLIDWORKS PDM Professional User Manager

*bsPasswd*
:   Password for bsUserName

*bsVaultName*
:   Vault name

Logs in to the specified vault using the specified user name and password.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Login( _    ByVal bsUserName As System.String, _    ByVal bsPasswd As System.String, _    ByVal bsVaultName As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Login(     System.string bsUserName,    System.string bsPasswd,    System.string bsVaultName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Login(  &   System.String^ bsUserName, &   System.String^ bsPasswd, &   System.String^ bsVaultName ) ``` | |

#### Parameters

*bsUserName*
:   User name of user created in the SOLIDWORKS PDM Professional User Manager

*bsPasswd*
:   Password for bsUserName

*bsVaultName*
:   Vault name

# ![](dotnetimages/collapse.gif)Remarks

If your application is custom (i.e., it is not supplied or supported by SOLIDWORKS PDM Professional) and your application:

* logs into SOLIDWORKS PDM Professional
  - or -* logs into a vault view
    - or -* directly accesses a vault database

when the same user is not already logged into a local view, you must first call [IEdmVault13::LoginEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault13~LoginEx.html) or [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html) to comply with the [SOLIDWORKS End User License Agreement (EULA)](http://www.solidworks.com/sw/eula.htm). Call IEdmVault13::LoginEx or IEdmVault5::LoginAuto before calling this method to ensure that licenses are properly consumed by your application.

Call IEdmVault5::LoginAuto to log in as a user already logged into a vault view through File Explorer or into a vault through the SOLIDWORKS PDM Professional client software. You do not need to specify a username and password when you call IEdmVault5::LoginAuto to share a license with the already logged-in user.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_ALREADY\_LOGGED\_IN: You are already logged into this vault.* E\_EDM\_LOGIN\_FAILED: You entered an invalid user name or password.* E\_EDM\_CANT\_OPEN\_DATABASE: The database could not be opened.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2