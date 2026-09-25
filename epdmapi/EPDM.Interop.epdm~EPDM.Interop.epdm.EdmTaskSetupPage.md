<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSetupPage.html -->

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

| EdmTaskSetupPage Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSetupPage_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmTaskSetupPage Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Used by the method [IEdmTaskProperties::SetSetupPages](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetSetupPages.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmTaskSetupPage     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmTaskSetupPage : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmTaskSetupPage : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmTaskSetupPage{
  string [mbsPageName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSetupPage~mbsPageName.html);
  integer [mlPageHwnd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSetupPage~mlPageHwnd.html);
  object [mpoPageImpl](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSetupPage~mpoPageImpl.html);
};

# ![](dotnetimages/collapse.gif)Example

[Create a Task that Finds Files in Workflow States (VB.NET)](Schedule_Task_to_Find_Files_in_State_Addin_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (C#)](Schedule_Task_to_Find_Files_in_State_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This structure defines a task add-in's setup page in the task properties dialog box.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmTaskSetupPage Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSetupPage_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[Programming Tasks](Tasks.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010