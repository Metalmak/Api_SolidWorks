<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo.html -->

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

| EdmBatchDelErrInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBatchDelErrInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about an error that occurred during execution of [IEdmBatchDelete::CommitDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~CommitDelete.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmBatchDelErrInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmBatchDelErrInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmBatchDelErrInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmBatchDelErrInfo{
  integer [mlDocID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo~mlDocID.html);
  integer [mlProjID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo~mlProjID.html);
  string [mbsPathName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo~mbsPathName.html);
  integer [mlErrorCode](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo~mlErrorCode.html);
};

# ![](dotnetimages/collapse.gif)Example

[Destroy Deleted Files in Vault (C#)](Destroy_Deleted_Files_in_Vault_Example_CSharp.htm)

[Destroy Deleted Files in Vault (VB.NET)](Destroy_Deleted_Files_in_Vault_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmBatchDelete3::GetCommitErrors](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3~GetCommitErrors.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmBatchDelErrInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 12.0 of SOLIDWORKS PDM Professional