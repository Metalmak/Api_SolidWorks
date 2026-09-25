<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~LogInWindowsUser.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| LogInWindowsUser Method (IEdmVault11) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html) : LogInWindowsUser Method (IEdmVault11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsUserName*
:   User name

*bsPasswd*
:   Password for bsUserName

*bsVaultName*
:   Name of vault to which to log in

Logs into SOLIDWORKS PDM Professional as the specified user.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub LogInWindowsUser( _    ByVal bsUserName As System.String, _    ByVal bsPasswd As System.String, _    ByVal bsVaultName As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void LogInWindowsUser(     System.string bsUserName,    System.string bsPasswd,    System.string bsVaultName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LogInWindowsUser(  &   System.String^ bsUserName, &   System.String^ bsPasswd, &   System.String^ bsVaultName ) ``` | |

#### Parameters

*bsUserName*
:   User name

*bsPasswd*
:   Password for bsUserName

*bsVaultName*
:   Name of vault to which to log in

# ![](dotnetimages/collapse.gif)Remarks

This method works like [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html), except this method does not display a login dialog box.

Any number of users can log in through the API, as long as they use the [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) method. However, only one user at a time can log in through the SOLIDWORKS PDM Professional client user interface. Both [IEdmVault11::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~LogInWindowsUser.html) and IEdmVault11::LogInWindowsUser log in the single user of the client user interface.

Call [IEdmVault11::GetLoggedInWindowsUserID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetLoggedInWindowsUserID.html) to obtain the ID of the user who is currently logged in through the client user interface.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_LOGIN\_FAILED: The specified user name or password is incorrect.* E\_EDM\_ALREADY\_LOGGED\_IN: Someone is already logged in from this client machine's user interface, or the IEdmVault object is already connected.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html)

[IEdmVault11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010