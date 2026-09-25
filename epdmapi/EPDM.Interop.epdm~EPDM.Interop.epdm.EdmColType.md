<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmColType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmColType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmColType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of file listing column content; specified in the [EdmListCol structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmColType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmColType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmColType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmCol\_AttachedVersion** | 10000 = As-built version |
| **EdmCol\_Category** | 12 = File category |
| **EdmCol\_Configuration** | 21 = Configuration name |
| **EdmCol\_Date** | 3 = File last modified date |
| **EdmCol\_EdmListRetFileFlag** | 30 = Combination of [EdmListRetFileFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListRetFileFlag.html) flags |
| **EdmCol\_FileSize** | 2 = File size |
| **EdmCol\_FileType** | 10 = File type |
| **EdmCol\_FoundInVersion** | 9 = Version in which the search tool found the file |
| **EdmCol\_LatestFileDate** | 17 = File latest version date |
| **EdmCol\_LatestVersion** | 4 = File latest version number |
| **EdmCol\_LockComputer** | 15 = Name of computer where the file is checked out |
| **EdmCol\_LockedIn** | 8 = Name of computer and folder path where the file is checked out |
| **EdmCol\_LockPath** | 14 = Path to folder where the file is checked out |
| **EdmCol\_LockUser** | 7 = Name of user who has the file checked out |
| **EdmCol\_LockUserID** | 13 = ID of user who has the file checked out |
| **EdmCol\_LockViewID** | 18 = ID of the file vault view where the file is checked out |
| **EdmCol\_Name** | 1 = File name |
| **EdmCol\_ParentFileConfiguration** | 29 = Name of the configuration referencing this file |
| **EdmCol\_ParentFileID** | 28 = ID of file referencing this file |
| **EdmCol\_Path** | 5 = File path |
| **EdmCol\_RefCount** | 11 = Reference count |
| **EdmCol\_Shared** | 19 = File share count |
| **EdmCol\_State** | 6 = File workflow state name + newline + file workflow state icon name |
| **EdmCol\_StateName** | 16 = File workflow state name |
| **EdmCol\_Variable** | 0 = The column is linked to a card variable |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)