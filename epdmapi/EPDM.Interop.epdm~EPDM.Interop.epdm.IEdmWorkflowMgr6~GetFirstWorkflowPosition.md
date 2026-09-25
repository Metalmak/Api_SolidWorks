<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6~GetFirstWorkflowPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstWorkflowPosition Method (IEdmWorkflowMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmWorkflowMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6.html) : GetFirstWorkflowPosition Method (IEdmWorkflowMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of all the workflows in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstWorkflowPosition() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstWorkflowPosition() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstWorkflowPosition(); ``` | |

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the first workflow in the enumeration

# ![](dotnetimages/collapse.gif)Example

See the [IEdmWorkflowMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, pass the returned position of the first workflow to [IEdmWorkflowMgr6::GetNextWorkflow](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6~GetNextWorkflow.html) to get the first workflow in this list. Then call IEdmWorkflowMgr6::GetNextWorkflow repeatedly to get the rest of the workflows.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmWorkflowMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6.html)

[IEdmWorkflowMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0