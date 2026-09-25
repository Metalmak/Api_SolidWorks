<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmSysPerm Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmSysPerm Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of system permissions for a user or group.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmSysPerm     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmSysPerm : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmSysPerm : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmSysPerm\_AcceptTasks** | 1026 = May accept tasks to execute on a host |
| **EdmSysPerm\_CanAddCustomColsInFileDetails** | 1032 = May add custom columns in File details |
| **EdmSysPerm\_CanAddCustomColsInFileOperations** | 1033 = May add custom columns in File operations |
| **EdmSysPerm\_CanAddDelLabels** | 2048 = May add and delete labels |
| **EdmSysPerm\_CanDeleteLabels** | 1029 = May delete labels |
| **EdmSysPerm\_CanPurgeHistory** | 1024 = May purge history listings |
| **EdmSysPerm\_CanSetLabels** | 1030 = May set labels |
| **EdmSysPerm\_CantIgnoreWarnings** | 4096 = Cannot click **OK** in the Check-in, Check-out, Get, etc., dialog boxes if there are any warnings in them |
| **EdmSysPerm\_CanUndoCheckOutAndCheckInForOthers** | 1028 =   1. May check in a file checked out to a different user in the same vault view- May undo checkouts of files that are checked out to a different user in the same or different vault view- Default permission for the Admin user in a new or upgraded 2018 vault- Applicable to all users/groups |
| **EdmSysPerm\_CanUpdateHistoryComments** | 1031 = May delete history comments |
| **EdmSysPerm\_EditAddins** | 4 = May install or uninstall add-ins |
| **EdmSysPerm\_EditReportQuery** | 512 = May modify report queries |
| **EdmSysPerm\_EditSharedSearchQuery** | 64 = May update shared search favorites |
| **EdmSysPerm\_EditTemplates** | 256 = May update templates |
| **EdmSysPerm\_EditUserMgr** | 1 = May update user and group properties |
| **EdmSysPerm\_EditWorkflow** | 2 = May edit workflows |
| **EdmSysPerm\_ExportWebFolder** | 128 = May export file vault folders to the internet |
| **EdmSysPerm\_MandatoryMailLogin** | 32 = Must enter password before sending email |
| **EdmSysPerm\_MandatoryStateComments** | 16 = Must enter change state comments |
| **EdmSysPerm\_MandatoryVersionComments** | 8 = Must enter version comments |
| **EdmSysPerm\_MaySeeAdminTool** | 67108864 = May see the Administration tool menu command item in File Explorer |
| **EdmSysPerm\_ModifyCardLists** | 131072 = May update definitions of lists used in cards |
| **EdmSysPerm\_ModifyCategories** | 8192 = May update category definitions |
| **EdmSysPerm\_ModifyColdStore** | 268435456 = May update the cold storage settings |
| **EdmSysPerm\_ModifyColumns** | 65536 = May update column definitions, including BOM definitions |
| **EdmSysPerm\_ModifyERPCfg** | 1073741824 = May update XML Import and Export settings |
| **EdmSysPerm\_ModifyIndexing** | 536870912 = May update the indexing settings |
| **EdmSysPerm\_ModifyItemNoGen** | 2097152 = May administrate items |
| **EdmSysPerm\_ModifyLicenseKey** | 524288 = May enter a new license key |
| **EdmSysPerm\_ModifyMailCfg** | 1048576 = May update the notification settings |
| **EdmSysPerm\_ModifyReplication** | 4194304 = May update vault replication settings |
| **EdmSysPerm\_ModifyRevisionNumbers** | 32768 = May update the definition of revision numbers |
| **EdmSysPerm\_ModifySearchForms** | 16777216 = May save search cards with the card editor |
| **EdmSysPerm\_ModifySerialNumbers** | 262144 = May update serial number generators |
| **EdmSysPerm\_ModifyTasks** | 1025 = May manage task definitions in the Administration tool |
| **EdmSysPerm\_ModifyTemplateForms** | 33554432 = May save template cards with the card editor |
| **EdmSysPerm\_ModifyToolbox** | 1027 = May update Toolbox Library settings in the Administration tool |
| **EdmSysPerm\_ModifyVariables** | 16384 = May update variable definitions |
| **EdmSysPerm\_None** | 0 = No rights at all |
| **EdmSysPerm\_RefuseLogin** | 134217728 = Block the user from logging in |

# ![](dotnetimages/collapse.gif)Remarks

This enumeration was added in SOLIDWORKS PDM Professional 2010 and supersedes the [EdmSysRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html) enumeration.

Always use the [IEdmUser7::HasSysRightEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser7~HasSysRightEx.html) and [IEdmUserGroup6::HasSysRightEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6~HasSysRightEx.html) methods instead of the obsoleted [IEdmUser5::HasSysRight](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5~HasSysRight.html) and [IEdmUserGroup5::HasSysRight](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5~HasSysRight.html) methods when writing code for SOLIDWORKS PDM Professional 2010 and later.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)