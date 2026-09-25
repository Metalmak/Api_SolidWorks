<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmWorkflow6 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmWorkflow6 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access a workflow set up using SOLIDWORKS PDM Professional's Workflow Editor.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmWorkflow6     Inherits IEdmObject5  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmWorkflow6 : IEdmObject5  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmWorkflow6 : public IEdmObject5  ``` | |

# ![](dotnetimages/collapse.gif)Example

[Create a Task that Finds Files in Workflow States (VB.NET)](Schedule_Task_to_Find_Files_in_State_Addin_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (C#)](Schedule_Task_to_Find_Files_in_State_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from [IEdmObject5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html) and supersedes [IEdmWorkflow5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow5.html).

Use [IEdmWorkflowMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6.html) to enumerate the installed workflows.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html)

[IEdmWorkflowMgr6::GetNextWorkflow](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6~GetNextWorkflow.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmWorkflow6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)