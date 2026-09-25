<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd.html -->

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

| EdmTaskMenuCmd Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmTaskMenuCmd Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Used by [IEdmTaskProperties::SetMenuCmds](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetMenuCmds.html) when an add-in adds menu commands to launch a task.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmTaskMenuCmd     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmTaskMenuCmd : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmTaskMenuCmd : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmTaskMenuCmd{
  integer [mlCmdID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd~mlCmdID.html)
  string [mbsMenuString](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd~mbsMenuString.html);
  integer [mlEdmMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd~mlEdmMenuFlags.html);
  string [mbsStatusBarHelp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd~mbsStatusBarHelp.html);
};

# ![](dotnetimages/collapse.gif)Example

[Create a Task that Finds Approved Files (VB.NET)](Schedule_Task_Addin_Example_VBNET.htm)

[Create a Task that Finds Approved Files (C#)](Schedule_Task_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmTaskMenuCmd Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[Programming Tasks](Tasks.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010