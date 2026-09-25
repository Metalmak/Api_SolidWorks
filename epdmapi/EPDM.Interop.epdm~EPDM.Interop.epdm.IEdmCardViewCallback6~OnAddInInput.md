<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6~OnAddInInput.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| OnAddInInput Method (IEdmCardViewCallback6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardViewCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html) : OnAddInInput Method (IEdmCardViewCallback6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFlags*
:   Combination of [EdmCardFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardFlag.html) bits from a button's add-in (see **Remarks**)

Handles input from an add-in when an add-in button is clicked in the card view.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub OnAddInInput( _    ByVal lFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void OnAddInInput(     System.int lFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnAddInInput(  &   System.int lFlags ) ``` | |

#### Parameters

*lFlags*
:   Combination of [EdmCardFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardFlag.html) bits from a button's add-in (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardViewCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

When an add-in's button is clicked in a card view, [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) is called. lFlags contains the same data that is returned in ppoData ([EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html)::mlLongData1) of IEdmAddIn5::OnCmd.

This method allows you to act on the information provided by the button's add-in.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardViewCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html)

[IEdmCardViewCallback6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0