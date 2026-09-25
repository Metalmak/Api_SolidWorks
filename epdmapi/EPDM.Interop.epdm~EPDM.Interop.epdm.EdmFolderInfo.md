<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo.html -->

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

| EdmFolderInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmFolderInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Information about a folder that is added to the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmFolderInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmFolderInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmFolderInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmFolderInfo{
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo~mlFolderID.html);
  string [mbsPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo~mbsPath.html);
  integer [mlParam](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo~mlParam.html);
  integer [mlEdmFolderInfoFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo~mlEdmFolderInfoFlags.html);
  [IEdmFolder6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6.html)\* [mpoFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo~mpoFolder.html);
};

# ![](dotnetimages/collapse.gif)Example

[Batch Add Folders (VB.NET)](Batch_Add_Folders_Example_VBNET.htm)

[Batch Add Folders (C#)](Batch_Add_Folders_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmBatchAddFolders::Create](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders~Create.html). One structure is returned for each folder added to the batch using [IEdmBatchAddFolders::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders~AddFolder.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmFolderInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional