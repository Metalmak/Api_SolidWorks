<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault14~InstallLicense2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| InstallLicense2 Method (IEdmVault14) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault14 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault14.html) : InstallLicense2 Method (IEdmVault14) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*brUserName*
:   Name of a SOLIDWORKS PDM Professional user

*bsPasswd*
:   Password for bsUserName

*bsVaultName*
:   Name of vault for which to install a license

*bsSNLServers*
:   Names of the port and server of the SolidNetwork License (SNL) server; for example, 25734@myserver

Installs a SOLIDWORKS PDM Professional license for this vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub InstallLicense2( _    ByVal brUserName As System.String, _    ByVal bsPasswd As System.String, _    ByVal bsVaultName As System.String, _    ByVal bsSNLServers As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void InstallLicense2(     System.string brUserName,    System.string bsPasswd,    System.string bsVaultName,    System.string bsSNLServers ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InstallLicense2(  &   System.String^ brUserName, &   System.String^ bsPasswd, &   System.String^ bsVaultName, &   System.String^ bsSNLServers ) ``` | |

#### Parameters

*brUserName*
:   Name of a SOLIDWORKS PDM Professional user

*bsPasswd*
:   Password for bsUserName

*bsVaultName*
:   Name of vault for which to install a license

*bsSNLServers*
:   Names of the port and server of the SolidNetwork License (SNL) server; for example, 25734@myserver

# ![](dotnetimages/collapse.gif)Remarks

In SOLIDWORKS PDM Professional:

* 2015 SP0 and later, licenses are shared among all vaults that use the same SolidNetwork License Server (SNL).* 2014 and earlier, licenses were shared among all vaults that were in the same SQL Server instance.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault14 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault14.html)

[IEdmVault14 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault14_members.html)

[IEdmVault11::GetLicense Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetLicense.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015