<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5~GetControl.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetControl Method (IEdmCard5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCard5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html) : GetControl Method (IEdmCard5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lControlID*
:   ID of card control to get

Gets a card control with the specified ID.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetControl( _    ByVal lControlID As System.Integer _ ) As IEdmCardControl5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmCardControl5 GetControl(     System.int lControlID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmCardControl5^ GetControl(  &   System.int lControlID ) ``` | |

#### Parameters

*lControlID*
:   ID of card control to get

#### Return Value

[IEdmCardControl5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_ID: The supplied control is invalid.* E\_EDM\_DATABASE\_ACCESS: The supplied control ID is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCard5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html)

[IEdmCard5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5_members.html)

[IEdmCard5::GetControlID Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5~GetControlID.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2