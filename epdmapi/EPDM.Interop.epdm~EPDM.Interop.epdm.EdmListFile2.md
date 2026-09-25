<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2.html -->

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

| EdmListFile2 Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmListFile2 Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Holds information about a file returned by the [IEdmBatchListing4::GetFiles2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing4~GetFiles2.html) method.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmListFile2     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmListFile2 : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmListFile2 : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmListFile

{
  short [mbHasLockRights](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mbHasLockRights.html);
  short [mbLocalOverwrittenVersionObsolete](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mbLocalOverwrittenVersionObsolete.html);
  string [mbsLockComputer](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mbsLockComputer.html);
  string [mbsLockPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mbsLockPath.html);
  string [mbsLockUser](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mbsLockUser.html);
  string [mbsLockViewID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mbsLockViewID.html);
  string [mbsRevisionName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mbsRevisionName.html);
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mlFileID.html);
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mlFolderID.html);
  integer [mlLatestVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mlLatestVersion.html);
  integer [mlLocalVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mlLocalVersion.html);
  integer [mlLockProjectID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mlLockProjectID.html);
  integer [mlParam](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mlParam.html);
  object [moColumnData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~moColumnData.html);
  struct [EdmWorkflowInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmWorkflowInfo.html) [moCurrentState](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~moCurrentState.html);
};

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This struct is an extended version of the [EdmListFile](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile.html) struct, which is returned by the [IEdmBatchListing::GetFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetFiles.html) method.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmListFile2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017