<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo.html -->

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

| EdmFileInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmFileInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Information about a file or folder that is added to or removed from the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmFileInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmFileInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmFileInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmFileInfo{
  integer [mlArg](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo~mlArg.html);
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo~mlFileID.html);
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo~mlFolderID.html);
  integer [mhResult](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo~mhResult.html);
  string [mbsPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo~mbsPath.html);
  IEdmObject5\* [mpoObject](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo~mpoObject.html);
};

# ![](dotnetimages/collapse.gif)Example

[Destroy Deleted Files in Vault (C#)](Destroy_Deleted_Files_in_Vault_Example_CSharp.htm)

[Destroy Deleted Files in Vault (VB.NET)](Destroy_Deleted_Files_in_Vault_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmBatchAdd::CommitAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~CommitAdd.html). One structure is returned for each file or folder added to the batch using one of the [IEdmBatchAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html)::AddXxxxx methods.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmFileInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional