<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmSysRightFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmSysRightFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [EdmSysPerm](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmSysRightFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmSysRightFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmSysRightFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmSysRight\_CanAddDelLabels** | 2048 = May add and delete labels |
| **EdmSysRight\_CanPurgeHistory** | 1024 = May delete the contents of history listings |
| **EdmSysRight\_CantIgnoreWarnings** | 4096 = May not click OK in the check in, check out, Get, etc. dialog boxes if there are warnings in them |
| **EdmSysRight\_EditAddins** | 4 = May install or uninstall add-ins |
| **EdmSysRight\_EditReportQuery** | 512 = May use the Report Generator |
| **EdmSysRight\_EditSharedSearchQuery** | 64 = May update shared search favorites |
| **EdmSysRight\_EditTemplates** | 256 = May run the Template Manager |
| **EdmSysRight\_EditUserMgr** | 1 = May run the User Manager |
| **EdmSysRight\_EditWorkflow** | 2 = May run the Workflow Editor |
| **EdmSysRight\_ExportWebFolder** | 128 = May export file vault folders to the internet |
| **EdmSysRight\_MandatoryMailLogin** | 32 = Must enter password before sending email |
| **EdmSysRight\_MandatoryStateComments** | 16 = Must enter change state comments |
| **EdmSysRight\_MandatoryVersionComments** | 8 = Must enter version comments |
| **EdmSysRight\_MaySeeAdminTool** | 67108864 = May see the Administration tool in the Tools menu in the File Explorer |
| **EdmSysRight\_ModifyCardLists** | 131072 = May update lists used in cards |
| **EdmSysRight\_ModifyCategories** | 8192 = May update category definitions in the SOLIDWORKS PDM Professional Administration tool |
| **EdmSysRight\_ModifyColdStore** | 268435456 = May update the cold storage settings |
| **EdmSysRight\_ModifyColumns** | 65536 = May update column definitions |
| **EdmSysRight\_ModifyERPCfg** | 1073741824 = May update ERP import/export settings |
| **EdmSysRight\_ModifyIndexing** | 536870912 = May update indexing settings |
| **EdmSysRight\_ModifyItemNoGen** | 2097152 = May update item settings |
| **EdmSysRight\_ModifyLicenseKey** | 524288 = May enter a new license key |
| **EdmSysRight\_ModifyMailCfg** | 1048576 = May update the notification settings |
| **EdmSysRight\_ModifyReplication** | 4194304 = May update replication settings |
| **EdmSysRight\_ModifyRevisionNumbers** | 32768 = May update the definition of revision numbers |
| **EdmSysRight\_ModifySearchForms** | 16777216 = May update search forms |
| **EdmSysRight\_ModifySerialNumbers** | 262144 = May update serial number generators |
| **EdmSysRight\_ModifyTemplateForms** | 33554432 = May update template input forms |
| **EdmSysRight\_ModifyVariables** | 16384 = May update variable definitions |
| **EdmSysRight\_None** | 0 = No permissions |
| **EdmSysRight\_RefuseLogin** | 134217728 = Block the user from logging in |

# ![](dotnetimages/collapse.gif)Remarks

Flags that indicate which SOLIDWORKS PDM Professional permissions a user has, etc. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)