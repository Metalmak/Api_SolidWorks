<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrokenParentInfo.html -->

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

| EdmBrokenParentInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrokenParentInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBrokenParentInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains broken parent information.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmBrokenParentInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmBrokenParentInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmBrokenParentInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmBrokenParentInfo{
  integer [mlParentFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrokenParentInfo~mlParentFileID.html);
  integer [mlParentFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrokenParentInfo~mlParentFolderID.html);
  string [mbsParentName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrokenParentInfo~mbsParentName.html);
  integer [mlChildFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrokenParentInfo~mlChildFileID.html);
  integer [mlChildFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrokenParentInfo~mlChildFolderID.html);
  string [mbsChildName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrokenParentInfo~mbsChildName.html);
};

# ![](dotnetimages/collapse.gif)See Also

####

[EdmBrokenParentInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrokenParentInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013