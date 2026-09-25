<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6~CreateCardViewEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateCardViewEx Method (IEdmVault6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6.html) : CreateCardViewEx Method (IEdmVault6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lEdmCardViewFlags*
:   Combination of [EdmCardViewFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewFlag.html) bits

*lCardID*
:   ID of card to display (see **Remarks**)

*lParentWindow*
:   Parent window handle

*lX*
:   X-position in pixels of the parent window

*lY*
:   Y-position in pixels of the parent window

*poCallback*
:   Pointer to a class that implements [IEdmCardViewCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html)

Obsolete. Superseded by [IEdmVault10::CreateCardViewEx2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10~CreateCardViewEx2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateCardViewEx( _    ByVal lEdmCardViewFlags As System.Integer, _    ByVal lCardID As System.Integer, _    ByVal lParentWindow As System.Integer, _    ByVal lX As System.Integer, _    ByVal lY As System.Integer, _    ByVal poCallback As IEdmCardViewCallback6 _ ) As IEdmCardView6 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmCardView6 CreateCardViewEx(     System.int lEdmCardViewFlags,    System.int lCardID,    System.int lParentWindow,    System.int lX,    System.int lY,    IEdmCardViewCallback6 poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmCardView6^ CreateCardViewEx(  &   System.int lEdmCardViewFlags, &   System.int lCardID, &   System.int lParentWindow, &   System.int lX, &   System.int lY, &   IEdmCardViewCallback6^ poCallback ) ``` | |

#### Parameters

*lEdmCardViewFlags*
:   Combination of [EdmCardViewFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewFlag.html) bits

*lCardID*
:   ID of card to display (see **Remarks**)

*lParentWindow*
:   Parent window handle

*lX*
:   X-position in pixels of the parent window

*lY*
:   Y-position in pixels of the parent window

*poCallback*
:   Pointer to a class that implements [IEdmCardViewCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html)

#### Return Value

[IEdmCardView6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView6.html)

# ![](dotnetimages/collapse.gif)Remarks

Use this method if you want complete control of the loading and saving of data to and from a custom file or folder data card. Use [IEdmFolder5::CreateCardView](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateCardView.html) if you want SOLIDWORKS PDM Professional to handle the loading and saving of data to and from a simple file or folder data card.

To obtain lCardID, call [IEdmVault6::GetCardID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6~GetCardID.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_ID: The specified card ID is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6.html)

[IEdmVault6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0