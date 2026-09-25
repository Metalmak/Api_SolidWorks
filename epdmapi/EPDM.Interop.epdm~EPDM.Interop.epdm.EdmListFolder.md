<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolder.html -->

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

| EdmListFolder Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolder_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmListFolder Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a folder returned from [IEdmBatchListing::GetFolders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetFolders.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmListFolder     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmListFolder : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmListFolder : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmListFolder{
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolder~mlFolderID.html);
  integer [mlParam](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolder~mlParam.html);
  string [mbsPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolder~mbsPath.html);
  object [moColumnData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolder~moColumnData.html);
};

# ![](dotnetimages/collapse.gif)See Also

####

[EdmListFolder Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolder_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional