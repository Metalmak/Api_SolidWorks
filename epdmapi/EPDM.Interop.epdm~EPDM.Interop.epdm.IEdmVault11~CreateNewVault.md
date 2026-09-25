<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~CreateNewVault.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateNewVault Method (IEdmVault11) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html) : CreateNewVault Method (IEdmVault11) |

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
:   Name of the vault to create

*bsDescription*
:   Description of the vault; appears in the vault properties window in the administration tool

*bsArchiveRootFolder*
:   Archive server vault folder; "" to use the default folder

*bsSQLServer*
:   Name or IP number of the SQL Server computer

*bsSQLUserName*
:   Name of the user who logs in to the SQL Server computer

*bsSQLPassword*
:   Password for the user who logs in to the SQL Server computer

*bsSQLDatabaseName*
:   Name of the SQL database for the new vault

*lDateFmt*
:   SQL Server date format code for the new vault (see **Remarks**)

*bsAdminUserPassword*
:   Password for the Admin user

*lEdmCreateVaultFlag*
:   Combination of [EdmCreateVaultFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCreateVaultFlag.html) bits

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to obtain progress information

*oExtra*
:   (see **Remarks**)

Creates a new vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CreateNewVault( _    ByVal bsArchiveServer As System.String, _    ByVal bsArchiveServerUserName As System.String, _    ByVal bsArchiveServerPassword As System.String, _    ByVal bsVaultName As System.String, _    ByVal bsDescription As System.String, _    ByVal bsArchiveRootFolder As System.String, _    ByVal bsSQLServer As System.String, _    ByVal bsSQLUserName As System.String, _    ByVal bsSQLPassword As System.String, _    ByVal bsSQLDatabaseName As System.String, _    ByVal lDateFmt As System.Integer, _    ByVal bsAdminUserPassword As System.String, _    ByVal lEdmCreateVaultFlag As System.Integer, _    ByVal poCallback As EdmCallback, _    Optional ByVal oExtra As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void CreateNewVault(     System.string bsArchiveServer,    System.string bsArchiveServerUserName,    System.string bsArchiveServerPassword,    System.string bsVaultName,    System.string bsDescription,    System.string bsArchiveRootFolder,    System.string bsSQLServer,    System.string bsSQLUserName,    System.string bsSQLPassword,    System.string bsSQLDatabaseName,    System.int lDateFmt,    System.string bsAdminUserPassword,    System.int lEdmCreateVaultFlag,    EdmCallback poCallback,    System.object oExtra ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CreateNewVault(  &   System.String^ bsArchiveServer, &   System.String^ bsArchiveServerUserName, &   System.String^ bsArchiveServerPassword, &   System.String^ bsVaultName, &   System.String^ bsDescription, &   System.String^ bsArchiveRootFolder, &   System.String^ bsSQLServer, &   System.String^ bsSQLUserName, &   System.String^ bsSQLPassword, &   System.String^ bsSQLDatabaseName, &   System.int lDateFmt, &   System.String^ bsAdminUserPassword, &   System.int lEdmCreateVaultFlag, &   EdmCallback^ poCallback, &   System.Object^ oExtra ) ``` | |

#### Parameters

*bsArchiveServer*
:   Name or IP number of the archive server computer; "" if the local comuter is the archive server

*bsArchiveServerUserName*
:   Name of the Windows user who logs in to the archive server

*bsArchiveServerPassword*
:   Password for the Windows user who logs in to the archive server

*bsVaultName*
:   Name of the vault to create

*bsDescription*
:   Description of the vault; appears in the vault properties window in the administration tool

*bsArchiveRootFolder*
:   Archive server vault folder; "" to use the default folder

*bsSQLServer*
:   Name or IP number of the SQL Server computer

*bsSQLUserName*
:   Name of the user who logs in to the SQL Server computer

*bsSQLPassword*
:   Password for the user who logs in to the SQL Server computer

*bsSQLDatabaseName*
:   Name of the SQL database for the new vault

*lDateFmt*
:   SQL Server date format code for the new vault (see **Remarks**)

*bsAdminUserPassword*
:   Password for the Admin user

*lEdmCreateVaultFlag*
:   Combination of [EdmCreateVaultFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCreateVaultFlag.html) bits

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to obtain progress information

*oExtra*
:   (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Create New Vault (VB.NET)](Create_New_Vault_Example_VBNET.htm)

[Create New Vault (C#)](Create_New_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

See the CAST/CONVERT documentation in the SQL Server online help to learn more about the date format codes for lDateFmt. The following table lists the valid values for lDateFmt:

| Date Codes | Date Format |
| --- | --- |
| 1 | 12/31/99 |
| 2 | 99.12.31 |
| 3 | 31/12/99 |
| 4 | 31.12.99 |
| 5 | 31-12-99 |
| 6 | 31 Dec 99 |
| 7 | Dec 31, 99 |
| 10 | 12-31-99 |
| 11 | 99/12/31 |
| 12 | 991231 |
| 102 | 1999.12.31 |
| 103 | 31/12/1999 |
| 104 | 31.12.1999 |
| 105 | 31-12-1999 |
| 106 | 31 Dec 1999 |
| 107 | Dec 31, 1999 |
| 110 | 12-31-1999 |
| 111 | 1999/12/31 |
| 112 | 19991231 |
| 120 | 1999-12-31 |

Specify oExtra with one of the following:

* VT\_BSTR containing either a CEX-file path to set up the vault with data from the export file or a valid vault configuration name like "Default", "Empty" or "SOLIDWORKS Quick Start"; for valid configuration names, see the **Configure Vault** step in the vault creation wizard of the administration tool* VT\_EMPTY to use default configuration

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_VAULT\_ALREADY\_EXISTS: There is already a file vault with the specified name on the archive server.* E\_EDM\_INVALID\_VAULT\_NAME: The vault name contains invalid characters or is longer than 31 characters. See the SOLIDWORKS PDM Professional administrative help for restrictions on valid characters in vault names.* E\_EDM\_ARCHIVE\_ROOT\_FOLDER\_DOES\_NOT\_EXIST: The root folder specified in bsArchiveRootFolder does not exist.* E\_EDM\_INVALID\_DATABASE\_NAME: The specified SQL database name is invalid. See the SOLIDWORKS PDM Professional administrative help or the Microsoft SQL Server help for restrictions regarding database names.* E\_EDM\_INSUFFICIENT\_SQL\_PERMISSION: The specified SQL user lacks permission to create a new database. (He or she must typically be a member of the sysadmin group.)* E\_EDM\_SQLSERVER\_UNSUPPORTED\_VERSION: The SQL server version is not supported. (SQL Server 2000 is not supported by SOLIDWORKS PDM Professional  2010.)* E\_EDM\_DATABASE\_ALREADY\_EXISTS: There is already an SQL database with the suggested name.* E\_EDM\_SQLSERVER\_LOGIN\_FAILED: The provided SQL credentials are not valid.* E\_EDM\_SQLSERVER\_CANNOT\_CONNECT: General failure connecting to the SQL-server machine. Maybe the name/IP contains a typo?* E\_EDM\_INVALID\_DATE\_FORMAT\_CODE: The lDateFmt argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html)

[IEdmVault11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11_members.html)

[IEdmVault11::CreateNewVaultView Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~CreateNewVaultView.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010