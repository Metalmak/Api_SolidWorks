<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2~GetAvailableTransitionList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetAvailableTransitionList Method (IEdmBatchChangeState2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchChangeState2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2.html) : GetAvailableTransitionList Method (IEdmBatchChangeState2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoTransitions*
:   Array of [EdmChangeStateTransitionInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo.html) structures; one structure for each state transition

Gets the state transitions available for the files in this batch.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetAvailableTransitionList( _    ByRef ppoTransitions() As EdmChangeStateTransitionInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetAvailableTransitionList(     out EdmChangeStateTransitionInfo[] ppoTransitions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetAvailableTransitionList(  &   [Out] array<EdmChangeStateTransitionInfo>^ ppoTransitions ) ``` | |

#### Parameters

*ppoTransitions*
:   Array of [EdmChangeStateTransitionInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo.html) structures; one structure for each state transition

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchChangeState2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchChangeState2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2.html)

[IEdmBatchChangeState2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013