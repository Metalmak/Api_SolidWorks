<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile.html -->

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

| EdmListFile Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmListFile Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Holds information about a file returned by the [IEdmBatchListing::GetFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetFiles.html) method.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmListFile     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmListFile : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmListFile : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmListFile

{
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~mlFileID.html);
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~mlFolderID.html);
  integer [mlParam](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~mlParam.html);
  integer [mlLatestVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~mlLatestVersion.html);
  integer [mlLocalVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~mlLocalVersion.html);
  string [mbsLockUser](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~mbsLockUser.html);
  string [mbsLockComputer](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~mbsLockComputer.html);
  string [mbsLockPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~mbsLockPath.html);
  string [mbsRevisionName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~mbsRevisionName.html);
  struct [EdmWorkflowInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmWorkflowInfo.html) [moCurrentState](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~moCurrentState.html);
  object [moColumnData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile~moColumnData.html);
};

# ![](dotnetimages/collapse.gif)Remarks

This struct is extended by [EdmListFile2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2.html), which is returned by the [IEdmBatchListing4::GetFiles2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing4~GetFiles2.html) method.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmListFile Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional