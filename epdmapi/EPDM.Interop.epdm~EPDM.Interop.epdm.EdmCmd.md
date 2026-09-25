<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html -->

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

| EdmCmd Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCmd Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains the kind of command issued and information common to all files and folders affected by the command.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmCmd     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmCmd : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmCmd : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmCmd{
   [enum EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html) [meCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~meCmdType.html);
   integer [mlParentWnd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mlParentWnd.html);
   integer [mlCurrentFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mlCurrentFolderID.html);
   integer [mlCmdID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mlCmdID.html);
   IEdmVault5 \*[mpoVault](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoVault.html);
   string [mbsComment](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbsComment.html);
   integer [mlEdmRefreshFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mlEdmRefreshFlags.html);
   object \*[mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html);
   boolean [mbSilentMode](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbSilentMode.html);
   boolean [mbCancel](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbCancel.html);
};

# ![](dotnetimages/collapse.gif)Example

[Notify User When File Changes State (VB.NET)](Notify_User_When_File_Changes_State_Example_VBNET.htm)

[Notify User When File Changes State (C#)](Notify_User_When_File_Changes_State_Example_CSharp.htm)

[Create a Task that Finds Approved Files (VB.NET)](Schedule_Task_Addin_Example_VBNET.htm)

[Create a Task that Finds Approved Files (C#)](Schedule_Task_Addin_Example_CSharp.htm)

[Change Card Variables Add-in (VB.NET)](Change_Card_Variables_Addin_Example_VBNET.htm)

[Change Card Variables Add-in (C#)](Change_Card_Variables_Addin_Example_CSharp.htm)

[Create a Task that Finds Files in Workflow States (VB.NET)](Schedule_Task_to_Find_Files_in_State_Addin_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (C#)](Schedule_Task_to_Find_Files_in_State_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by reference when an add-in's [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) is called by SOLIDWORKS PDM Professional.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmCmd Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional