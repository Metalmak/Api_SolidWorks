<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6~GetTransition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetTransition Method (IEdmWorkflow6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmWorkflow6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6.html) : GetTransition Method (IEdmWorkflow6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lTransitionID*
:   ID of workflow state transition to get

Gets the workflow state transition with the specified ID.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetTransition( _    ByVal lTransitionID As System.Integer _ ) As IEdmTransition6 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmTransition6 GetTransition(     System.int lTransitionID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmTransition6^ GetTransition(  &   System.int lTransitionID ) ``` | |

#### Parameters

*lTransitionID*
:   ID of workflow state transition to get

#### Return Value

[IEdmTransition6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition6.html)

# ![](dotnetimages/collapse.gif)Remarks

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmTransition6.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_ID: lTransitionID is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmWorkflow6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6.html)

[IEdmWorkflow6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0