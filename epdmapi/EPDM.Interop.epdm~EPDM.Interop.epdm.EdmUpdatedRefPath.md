<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUpdatedRefPath.html -->

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

| EdmUpdatedRefPath Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUpdatedRefPath_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUpdatedRefPath Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains old and new path information for references that are moved or renamed by another client.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmUpdatedRefPath     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmUpdatedRefPath : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmUpdatedRefPath : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmUpdatedRefPath{
  string [mbsRefOldPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUpdatedRefPath~mbsRefOldPath.html);
  string [mbsRefNewPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUpdatedRefPath~mbsRefNewPath.html);
};

# ![](dotnetimages/collapse.gif)Remarks

This structure is returned by [IEdmRefItem2::GetUpdatedPaths](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem2~GetUpdatedPaths.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmUpdatedRefPath Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUpdatedRefPath_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021 SP04