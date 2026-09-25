<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5~GetValidation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetValidation Method (IEdmCardControl5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardControl5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html) : GetValidation Method (IEdmCardControl5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poMin*
:   Minimum limit; minimum number of characters in a control of type, EdmVariableType.EdmVarType\_Text

*poMax*
:   Maximum limit for this control's value; maximum number of characters in a control of type, EdmVariableType.EdmVarType\_Text

Gets the input validation criteria for this control.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetValidation( _    ByRef poMin As System.Object, _    ByRef poMax As System.Object _ ) As EdmVariableType ``` | |

| C# |  |
| --- | --- |
| ``` EdmVariableType GetValidation(     out System.object poMin,    out System.object poMax ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmVariableType GetValidation(  &   [Out] System.Object^ poMin, &   [Out] System.Object^ poMax ) ``` | |

#### Parameters

*poMin*
:   Minimum limit; minimum number of characters in a control of type, EdmVariableType.EdmVarType\_Text

*poMax*
:   Maximum limit for this control's value; maximum number of characters in a control of type, EdmVariableType.EdmVarType\_Text

#### Return Value

Data type to validate as defined in [EdmVariableType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableType.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardControl6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

If a card control has input validation, the user is unable to click **OK** or **Apply** until all validation conditions are met.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardControl5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html)

[IEdmCardControl5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2