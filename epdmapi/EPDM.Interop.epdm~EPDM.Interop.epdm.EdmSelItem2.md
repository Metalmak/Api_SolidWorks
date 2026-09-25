<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2.html -->

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

| EdmSelItem2 Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmSelItem2 Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a selected item.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmSelItem2     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmSelItem2 : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmSelItem2 : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmSelItem2

{
    [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2~meType.html);

    integer [mlID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2~mlID.html);
    integer [mlParentID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2~mlParentID.html);
    integer [mlVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2~mlVersion.html);
};

# ![](dotnetimages/collapse.gif)Example

[Create a Task that Finds Approved Files (VB.NET)](Schedule_Task_Addin_Example_VBNET.htm)

[Create a Task that Finds Approved Files (C#)](Schedule_Task_Addin_Example_CSharp.htm)

[Create a Task that Finds Files in Workflow States (VB.NET)](Schedule_Task_to_Find_Files_in_State_Addin_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (C#)](Schedule_Task_to_Find_Files_in_State_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Used by:

* oNotificationAttachments argument of [IEdmTaskInstance::SetStatus](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetStatus.html).* poSelections argument of [IEdmTaskMgr::RunTask](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskMgr~RunTask.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmSelItem2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010