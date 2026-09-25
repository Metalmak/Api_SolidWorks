<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html -->

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

| EdmHistoryItem Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmHistoryItem Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains a history item.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmHistoryItem     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmHistoryItem : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmHistoryItem : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmHistoryItem{
  [enum EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~meType.html);
  datetime [moDate](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~moDate.html);
  integer [mlVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~mlVersion.html);
  integer [mlUserID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~mlUserID.html);
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~mlFileID.html);
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~mlFolderID.html);
  string [mbsItemName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~mbsItemName.html);
  string [mbsUserName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~mbsUserName.html);
  string [mbsComment](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~mbsComment.html);
  [struct EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html) [moData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem~moData.html);
};

# ![](dotnetimages/collapse.gif)Example

[Get Histories of Files (VB.NET)](Get_Histories_of_Files_Example_VBNET.htm)

[Get Histories of Files (C#)](Get_Histories_of_Files_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmHistory](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmHistoryItem Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional