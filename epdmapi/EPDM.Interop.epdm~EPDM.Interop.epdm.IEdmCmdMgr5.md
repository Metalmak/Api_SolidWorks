<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmCmdMgr5 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmCmdMgr5 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to add menu commands, toolbar buttons, and command hooks to SOLIDWORKS PDM Professional.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmCmdMgr5 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmCmdMgr5 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmCmdMgr5 ``` | |

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

This interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* is extended by [IEdmCmdMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr6.html).

A pointer to this interface is provided by SOLIDWORKS PDM Professional when it loads an add-in. [IEdmAddIn5::GetAddInInfo's](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html) poCmdMgr contains a pointer to this interface. Within your implementation of IEdmAddIn5::GetAddInInfo, use this pointer to call:

* [IEdmCmdMgr5::AddCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddCmd.html) to add menu commands* [IEdmCmdMgr5::AddToolbarImage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddToolbarImage.html) to add toolbar buttons* [IEdmCmdMgr5::AddHook](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddHook.html) to add command hooks

to SOLIDWORKS PDM Professional.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCmdMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[Creating Menu Commands (VB.NET)](vbmenuitem.htm)

[Creating Add-in Hooks (VB.NET)](vbreactor.htm)