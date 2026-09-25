<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5~GetButtonCommand.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetButtonCommand Method (IEdmCardControl5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardControl5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html) : GetButtonCommand Method (IEdmCardControl5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

Gets the command string that is executed when a button is clicked in the Card Editor.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetButtonCommand( _    ByVal lParentWnd As System.Integer _ ) As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetButtonCommand(     System.int lParentWnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetButtonCommand(  &   System.int lParentWnd ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

#### Return Value

Command string

# ![](dotnetimages/collapse.gif)Remarks

If the button is linked to a program that is not found, this method launches a dialog box in which the user can browse to the missing EXE file. If the user clicks **Cancel** in the dialog box, HRESULT = E\_EDM\_CANCELLED\_BY\_USER is returned by this method.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_ID: The supplied control is not a push-button. Call [IEdmCardControl5::ControlType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5~ControlType.html) first to verify whether the control is a push-button.* E\_EDM\_CANCELLED\_BY\_USER: The user clicked **Cancel** in the dialog box.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardControl5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html)

[IEdmCardControl5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2