<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumnType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmBomColumnType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBomColumnType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of Bill of Material (BOM) column content; specified in [EdmBomColumn](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn.html) and in calls to [IEdmBomCell:GetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell~GetVar.html), and [IEdmBomCell::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell~SetVar.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmBomColumnType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmBomColumnType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmBomColumnType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmBomCol\_Configuration** | 21 = Name of the current configuration |
| **EdmBomCol\_Date** | 3 = Modified date of file |
| **EdmBomCol\_DocType** | 12 = Document |
| **EdmBomCol\_FileSize** | 2 = File size in bytes |
| **EdmBomCol\_FileType** | 10 = File type |
| **EdmBomCol\_FoundInVersion** | 9 = Version where found |
| **EdmBomCol\_ID** | 23 = File ID |
| **EdmBomCol\_LatestFileDate** | 17 = File date of the latest version |
| **EdmBomCol\_LatestVersion** | 4 = Latest version number of the file |
| **EdmBomCol\_LockDomain** | 15 = Name of computer where file is checked out |
| **EdmBomCol\_LockedIn** | 8 = Computer name and path of checked-out file |
| **EdmBomCol\_LockPath** | 14 = File path of checked-out file |
| **EdmBomCol\_LockUser** | 7 = Name of user who has checked out the file |
| **EdmBomCol\_LockUserID** | 13 = ID of user who has checked out the file |
| **EdmBomCol\_LockViewID** | 18 = ID of vault view where file is checked out |
| **EdmBomCol\_Name** | 1 = File or folder name |
| **EdmBomCol\_PartNumber** | 24 = Document name, configuration name, or user-specified name; used in BOM lists |
| **EdmBomCol\_Path** | 5 = Path to file folder |
| **EdmBomCol\_RefCount** | 11 = Reference count or BOM Quantity |
| **EdmBomCol\_RefCountNoBomQty** | 25 = Reference count that is not multiplied by BOM quantity |
| **EdmBomCol\_RefVariable** | 22 = Variable set on a reference to the file, e.g., position number, cut length, etc. |
| **EdmBomCol\_Shared** | 19 = Number of folders in which the file is shared |
| **EdmBomCol\_State** | 6 = File workflow state name + new line + file workflow state icon name |
| **EdmBomCol\_StateName** | 16 = File workflow state name |
| **EdmBomCol\_Variable** | 0 = This column is linked to a card variable |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)