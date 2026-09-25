<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~InstallLicense.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| InstallLicense Method (IEdmVault11) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html) : InstallLicense Method (IEdmVault11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsUserName*
:   Name of a SOLIDWORKS PDM Professional user

*bsPasswd*
:   Password for bsUserName

*bsVaultName*
:   Name of vault for which to install a license

*bsLicenseFilePath*
:   Path to the license file

Obsolete. Replaced by [IEdmVault14::InstallLicense2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault14~InstallLicense2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub InstallLicense( _    ByVal bsUserName As System.String, _    ByVal bsPasswd As System.String, _    ByVal bsVaultName As System.String, _    ByVal bsLicenseFilePath As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void InstallLicense(     System.string bsUserName,    System.string bsPasswd,    System.string bsVaultName,    System.string bsLicenseFilePath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InstallLicense(  &   System.String^ bsUserName, &   System.String^ bsPasswd, &   System.String^ bsVaultName, &   System.String^ bsLicenseFilePath ) ``` | |

#### Parameters

*bsUserName*
:   Name of a SOLIDWORKS PDM Professional user

*bsPasswd*
:   Password for bsUserName

*bsVaultName*
:   Name of vault for which to install a license

*bsLicenseFilePath*
:   Path to the license file

# ![](dotnetimages/collapse.gif)Remarks

In SOLIDWORKS PDM Professional 2014 and earlier, licenses were shared among all vaults that were in the same SQL Server instance. Because licenses are shared among all vaults that use the same SolidNetwork License Server (SNL) in SOLIDWORKS PDM Professional 2015 SP0 and later, this method is obsolete and replaced by [IEdmVault14::InstallLicense2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault14~InstallLicense2.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html)

[IEdmVault11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010