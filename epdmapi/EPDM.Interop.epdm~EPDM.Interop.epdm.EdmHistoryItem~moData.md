<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~moData.html -->

![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/drpdown.gif)
![](dotnetimages/drpdown_orange.gif)
![](dotnetimages/copycode.gif)
![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |

| moData Field | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [EdmHistoryItem Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html) : moData Field |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Extra data.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public moData As EdmCmdData ``` | |

| C# |  |
| --- | --- |
| ``` public EdmCmdData moData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public: EdmCmdData moData ``` | |

#### Field Value

[EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html) structure whose content depends on [EdmHistoryItem::meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~meType.html) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

The members of the structure stored in this member have different values, depending on the value of EdmHistoryItem::meType. The tables below contain the moData structure member values for each EdmHistoryItem::meType. Any members not listed in the tables are undefined for that data type.

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileShare

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Destination folder path |
| mlObjectID1 | Destination folder ID |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileRename

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Old file name |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileMove

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Source folder path |
| mbsStrData2 | Destination folder path |
| mlObjectID1 | Source folder ID |
| mlObjectID2 | Destination folder ID |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileRollback

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mlLongData1 | From version |
| mlLongData2 | To version |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileDelete

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mlObjectID1 | Parent folder ID |
| mbsStrData1 | Parent folder path |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileUndelete

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mlObjectID1 | Parent folder ID |
| mbsStrData1 | Parent folder path |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileLabel

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Label name |
| mlObjectID1 | Label ID |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileState

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Source workflow name + <newline> + source state name |
| mbsStrData2 | Destination workflow name + <newline> + destination state name |
| mlLongData1 | Transition number |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileRevision

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Revision name |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FileColdStore

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Media name |
| mlLongData1 | Storage type |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FolderDelete

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Folder path |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FolderUndelete

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Folder path |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FolderCreate

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Folder path |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FolderCardData

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Folder path |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FolderRename

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Old folder name |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FolderMove

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | From folder path |
| mbsStrData2 | To folder path |
| mlObjectID1 | From folder ID |
| mlObjectID2 | To folder ID |

#### EdmHistoryItem::meType = [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html).Edmhist\_FolderLabel

|  |  |
| --- | --- |
| **EdmCmdData Members** | **Description** |
| mbsStrData1 | Label name |
| mlObjectID1 | Label ID |

# ![](dotnetimages/collapse.gif)See Also

####

[EdmHistoryItem Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html)

[EdmHistoryItem Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem_members.html)