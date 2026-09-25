<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~CreateNewVaultView.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateNewVaultView Method (IEdmVault11) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html) : CreateNewVaultView Method (IEdmVault11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsArchiveServer*
:   Name or IP number of the archive server computer; "" if the local comuter is the archive server

*bsArchiveServerUserName*
:   Name of the Windows user who logs in to the archive server

*bsArchiveServerPassword*
:   Password for the Windows user who logs in to the archive server

*bsVaultName*
:   Name of the vault for which to create a view

*bsParentFolderPath*
:   Full system path to the parent folder of the view; a subfolder with the same name as the vault is created in the parent folder

*lEdmCreateVaultViewFlag*
:   Combination of [EdmCreateVaultViewFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCreateVaultViewFlag.html) bits

Creates a local view of a file vault in File Explorer.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CreateNewVaultView( _    ByVal bsArchiveServer As System.String, _    ByVal bsArchiveServerUserName As System.String, _    ByVal bsArchiveServerPassword As System.String, _    ByVal bsVaultName As System.String, _    ByVal bsParentFolderPath As System.String, _    ByVal lEdmCreateVaultViewFlag As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void CreateNewVaultView(     System.string bsArchiveServer,    System.string bsArchiveServerUserName,    System.string bsArchiveServerPassword,    System.string bsVaultName,    System.string bsParentFolderPath,    System.int lEdmCreateVaultViewFlag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CreateNewVaultView(  &   System.String^ bsArchiveServer, &   System.String^ bsArchiveServerUserName, &   System.String^ bsArchiveServerPassword, &   System.String^ bsVaultName, &   System.String^ bsParentFolderPath, &   System.int lEdmCreateVaultViewFlag ) ``` | |

#### Parameters

*bsArchiveServer*
:   Name or IP number of the archive server computer; "" if the local comuter is the archive server

*bsArchiveServerUserName*
:   Name of the Windows user who logs in to the archive server

*bsArchiveServerPassword*
:   Password for the Windows user who logs in to the archive server

*bsVaultName*
:   Name of the vault for which to create a view

*bsParentFolderPath*
:   Full system path to the parent folder of the view; a subfolder with the same name as the vault is created in the parent folder

*lEdmCreateVaultViewFlag*
:   Combination of [EdmCreateVaultViewFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCreateVaultViewFlag.html) bits

# ![](dotnetimages/collapse.gif)Example

[Create New Vault (VB.NET)](Create_New_Vault_Example_VBNET.htm)

[Create New Vault (C#)](Create_New_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_FOLDER\_NOT\_FOUND: The parent folder does not exist.* E\_EDM\_VERSION\_MISMATCH: The client version and the archive server version do not match.* E\_EDM\_FVC\_CANT\_WRITE\_TO\_REGISTRY: Failed to write to the system registry. Possibly you are trying to create a shared view, and the logged-in Windows user lacks privileges to write to HKEY\_LOCAL\_MACHINE.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html)

[IEdmVault11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11_members.html)

[IEdmVault11::CreateNewVault Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~CreateNewVault.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010