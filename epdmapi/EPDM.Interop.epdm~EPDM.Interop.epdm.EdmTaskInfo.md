<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskInfo.html -->

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

| EdmTaskInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmTaskInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Used by [IEdmTaskMgr::RunTask](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskMgr~RunTask.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmTaskInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmTaskInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmTaskInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmTaskInfo{
  string [mbsTaskName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskInfo~mbsTaskName.html);
  long [mllShortTaskInfoFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskInfo~mllShortTaskInfoFlags.html);
  integer [mlTaskID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskInfo~mlTaskID.html);
};

# ![](dotnetimages/collapse.gif)See Also

####

[EdmTaskInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[Programming Tasks](Tasks.htm)