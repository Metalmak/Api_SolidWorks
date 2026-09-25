<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo.html -->

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

| EdmGenItemInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGenItemInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about generated items.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmGenItemInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmGenItemInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmGenItemInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmGenItemInfo{
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mlFileID.html);
  integer [mlFileParentFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mlFileParentFolderID.html);
  string [mbsConfiguration](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mbsConfiguration.html);
  integer [mlFileVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mlFileVersion.html);
  string [mbsFileFolderPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mbsFileFolderPath.html);
  string [mbsFileName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mbsFileName.html);
  integer [mlItemID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mlItemID.html);
  integer [mlItemParentFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mlItemParentFolderID.html);
  [enum EdmItemLinkType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemLinkType.html) [meLinkType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~meLinkType.html);
  string [mbsItemFolderPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mbsItemFolderPath.html);
  string [mbsItemName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mbsItemName.html);
  string [mbsItemAlternativeName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mbsItemAlternativeName.html);
  integer [mhResult](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo~mhResult.html);
};

# ![](dotnetimages/collapse.gif)Example

[Add Items (C#)](Add_Items_Example_CSharp.htm)

[Add Items (VB.NET)](Add_Items_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmBatchItemGeneration::GenerateItems](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~GenerateItems.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmGenItemInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010