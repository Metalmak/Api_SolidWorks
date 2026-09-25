<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmAddIn5 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmAddIn5 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to create a SOLIDWORKS PDM Professional add-in.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmAddIn5 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmAddIn5 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmAddIn5 ``` | |

# ![](dotnetimages/collapse.gif)Example

See [Add-in Applications](AddInApp.htm).

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

This interface inherits from IUnknown. See [Using and Implementing IUnknown (COM)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms693423%28v%3Dvs.85%29.aspx).

To create a SOLIDWORKS PDM Professional add-in:

1. Create a class that implements this interface and its methods.- Add menu commands, toolbar buttons, and hooks in your implementation of [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html).- Add callbacks for the hooks, menu commands, and toolbar buttons in your implementation of [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html).- Register the add-in via the [Administration Add-ins dialog](AdminDlg.htm). During registration, SOLIDWORKS PDM Professional calls your IEdmAddIn5::GetAddInInfo method to obtain information about the add-in.

After the add-in is created and registered, SOLIDWORKS PDM Professional calls your IEdmAddIn5::OnCmd method whenever the user executes a menu command or hook from your add-in.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddIn5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmAddInDrawButton5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5.html)