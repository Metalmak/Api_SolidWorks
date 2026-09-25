<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault13~LoginEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| LoginEx Method (IEdmVault13) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault13 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault13.html) : LoginEx Method (IEdmVault13) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsUserName*
:   User name of user created in the SOLIDWORKS PDM Professional User Manager

*bsPasswd*
:   User password for bsUserName

*bsVaultName*
:   Name of vault

*lEdmLoginFlags*
:   Login flags:

    * 0 = Nothing* 1 = Web client

Allows an application that is not supplied and supported by SOLIDWORKS Corporation to:

* log into SOLIDWORKS PDM Professional
  - or -* log into a vault view
    - or -* directly access the vault database

when the same user is not already logged into a local view.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub LoginEx( _    ByVal bsUserName As System.String, _    ByVal bsPasswd As System.String, _    ByVal bsVaultName As System.String, _    Optional ByVal lEdmLoginFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void LoginEx(     System.string bsUserName,    System.string bsPasswd,    System.string bsVaultName,    System.int lEdmLoginFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LoginEx(  &   System.String^ bsUserName, &   System.String^ bsPasswd, &   System.String^ bsVaultName, &   System.int lEdmLoginFlags ) ``` | |

#### Parameters

*bsUserName*
:   User name of user created in the SOLIDWORKS PDM Professional User Manager

*bsPasswd*
:   User password for bsUserName

*bsVaultName*
:   Name of vault

*lEdmLoginFlags*
:   Login flags:

    * 0 = Nothing* 1 = Web client

# ![](dotnetimages/collapse.gif)Remarks

To make it easier to program and to comply with the [SOLIDWORKS End User License Agreement (EULA)](http://www.solidworks.com/sw/eula.htm), this method ensures that licenses are properly consumed by your application.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault13 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault13.html)

[IEdmVault13 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault13_members.html)

[IEdmVault5::Login Method()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html)

[IEdmVault5::LoginAuto Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2014