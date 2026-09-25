<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef.html -->

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

| EdmCheckRef Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCheckRef Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a file reference.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmCheckRef     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmCheckRef : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmCheckRef : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmCheckRef{
  integer [mlParentFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef~mlParentFileID.html);
  integer [mlRefFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef~mlRefFileID.html);
  string [mbsParentPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef~mbsParentPath.html);
  string [mbsRefPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef~mbsRefPath.html);
  integer [mlRefVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef~mlRefVersion.html);
  integer [mlRefLatestVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef~mlRefLatestVersion.html);
  integer [mlRefFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef~mlRefFolderID.html);
};

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmRevisionMgr3::VerUpgrade\_ReferenceCheck](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr3~VerUpgrade_ReferenceCheck.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmCheckRef Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009