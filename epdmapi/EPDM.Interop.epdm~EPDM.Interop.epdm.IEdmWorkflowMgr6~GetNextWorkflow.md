<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6~GetNextWorkflow.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextWorkflow Method (IEdmWorkflowMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmWorkflowMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6.html) : GetNextWorkflow Method (IEdmWorkflowMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next workflow in the list

Gets the next workflow in an enumeration.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextWorkflow( _    ByVal poPos As IEdmPos5 _ ) As IEdmWorkflow6 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmWorkflow6 GetNextWorkflow(     IEdmPos5 poPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmWorkflow6^ GetNextWorkflow(  &   IEdmPos5^ poPos ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next workflow in the list

#### Return Value

[IEdmWorkflow6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmWorkflowMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPos with the interface to the position of the first workflow in the list, IEdmPos5. Call [IEdmWorkflowMgr6::GetFirstWorkflowPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6~GetFirstWorkflowPosition.html) to obtain poPos.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the workflows in the list.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmWorkflow6.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmWorkflowMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6.html)

[IEdmWorkflowMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflowMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0