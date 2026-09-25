<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel.html -->

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

| EdmTaskSel Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmTaskSel Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Passed as argument to [IEdmTaskProperties::SetSel](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetSel.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmTaskSel     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmTaskSel : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmTaskSel : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmTaskSel{
  [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel~meType.html);
  integer [mlID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel~mlID.html);
  integer [mlParentID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel~mlParentID.html);
  integer [mlVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel~mlVersion.html);
  string [mbsConfiguration](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel~mbsConfiguration.html);
};

# ![](dotnetimages/collapse.gif)Remarks

The struct contains a selected item that should be processed by the task.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmTaskSel Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[Programming Tasks](Tasks.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010