<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5~GetControlID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetControlID Method (IEdmCard5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCard5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html) : GetControlID Method (IEdmCard5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVariableNameOrID*
:   ID or name of the variable for which to get the control ID

Gets the ID of the control that is connected to the specified variable in this card.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetControlID( _    ByRef poVariableNameOrID As System.Object _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetControlID(     ref System.object poVariableNameOrID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetControlID(  &   System.Object^% poVariableNameOrID ) ``` | |

#### Parameters

*poVariableNameOrID*
:   ID or name of the variable for which to get the control ID

#### Return Value

Control ID; 0 if the variable isn't used by any control in this card

# ![](dotnetimages/collapse.gif)Remarks

If more than one control is connected to the same variable, there is no way of knowing for which control this method returns an ID.

The returned ID can be passed to [IEdmCard5::GetControl](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5~GetControl.html) or [IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html) in order to obtain [IEdmCardControl5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The variable was not found.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCard5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html)

[IEdmCard5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2