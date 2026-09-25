<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6~GetCtrlData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCtrlData Method (IEdmCardViewCallback6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardViewCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html) : GetCtrlData Method (IEdmCardViewCallback6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lCardWnd*
:   Window handle of the card

*lCardID*
:   ID of the card (see **Remarks**)

*lControlID*
:   ID of the control for which to get the value (see **Remarks**)

*lVariableID*
:   ID of the variable used by this control (see **Remarks**)

*bsVariableName*
:   Name of the variable used by this control

*poView*
:   [IEdmCardView5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView5.html)

Gets the data to insert into a control when a card is opened.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetCtrlData( _    ByVal lCardWnd As System.Integer, _    ByVal lCardID As System.Integer, _    ByVal lControlID As System.Integer, _    ByVal lVariableID As System.Integer, _    ByVal bsVariableName As System.String, _    ByVal poView As IEdmCardView5 _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetCtrlData(     System.int lCardWnd,    System.int lCardID,    System.int lControlID,    System.int lVariableID,    System.string bsVariableName,    IEdmCardView5 poView ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetCtrlData(  &   System.int lCardWnd, &   System.int lCardID, &   System.int lControlID, &   System.int lVariableID, &   System.String^ bsVariableName, &   IEdmCardView5^ poView ) ``` | |

#### Parameters

*lCardWnd*
:   Window handle of the card

*lCardID*
:   ID of the card (see **Remarks**)

*lControlID*
:   ID of the control for which to get the value (see **Remarks**)

*lVariableID*
:   ID of the variable used by this control (see **Remarks**)

*bsVariableName*
:   Name of the variable used by this control

*poView*
:   [IEdmCardView5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView5.html)

#### Return Value

Data for the specified control

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardViewCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The framework calls this method once per control when a card created with [IEdmVault10::CreateCardViewEx2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10~CreateCardViewEx2.html) is opened.

| Use... | In a call to [IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html) with eType = ... | To obtain... |
| --- | --- | --- |
| ICardID | [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html).EdmObject\_Card | [IEdmCard5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html) |
| IControlID | EdmObjectType.EdmObject\_CardControl | [IEdmCardControl5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html) |
| IVariableID | EdmObjectType.EdmObject\_Variable | [IEdmVariable5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5.html) |

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardViewCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html)

[IEdmCardViewCallback6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0