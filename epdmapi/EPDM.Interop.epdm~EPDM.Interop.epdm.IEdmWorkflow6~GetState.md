<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6~GetState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetState Method (IEdmWorkflow6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmWorkflow6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6.html) : GetState Method (IEdmWorkflow6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poIdOrName*
:   ID or name of workflow state to get

Gets the workflow state with the specified ID or name.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetState( _    ByRef poIdOrName As System.Object _ ) As IEdmState6 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmState6 GetState(     ref System.object poIdOrName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmState6^ GetState(  &   System.Object^% poIdOrName ) ``` | |

#### Parameters

*poIdOrName*
:   ID or name of workflow state to get

#### Return Value

[IEdmState6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState6.html); Null if poIdOrName is invalid

# ![](dotnetimages/collapse.gif)Remarks

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmState6.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: poIdOrName contains an invalid name.* E\_EDM\_INVALID\_ID: poIdOrName contain an invalid ID.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmWorkflow6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6.html)

[IEdmWorkflow6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0