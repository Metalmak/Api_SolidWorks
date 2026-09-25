<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView61~SetFocus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetFocus Method (IEdmCardView61) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardView61 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView61.html) : SetFocus Method (IEdmCardView61) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVariableNameOrID*
:   Name or ID of the variable to which to set focus; 0 to set focus to the first control in the card

Sets input focus to a certain control in this card view.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetFocus( _    Optional ByRef poVariableNameOrID As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFocus(     ref System.object poVariableNameOrID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFocus(  &   System.Object^% poVariableNameOrID ) ``` | |

#### Parameters

*poVariableNameOrID*
:   Name or ID of the variable to which to set focus; 0 to set focus to the first control in the card

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardView61](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView61.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardView61 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView61.html)

[IEdmCardView61 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView61_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0