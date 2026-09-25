<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10~CreateCardViewEx2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateCardViewEx2 Method (IEdmVault10) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10.html) : CreateCardViewEx2 Method (IEdmVault10) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poArgs*
:   [EdmCardViewParams](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams.html) structure containing various members that control the creation of the view

*poCallback*
:   Pointer to a class that implements [IEdmCardViewCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html)

Displays a file or folder data card.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateCardViewEx2( _    ByRef poArgs As EdmCardViewParams, _    ByVal poCallback As System.Object _ ) As IEdmCardView63 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmCardView63 CreateCardViewEx2(     ref EdmCardViewParams poArgs,    System.object poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmCardView63^ CreateCardViewEx2(  &   EdmCardViewParams% poArgs, &   System.Object^ poCallback ) ``` | |

#### Parameters

*poArgs*
:   [EdmCardViewParams](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams.html) structure containing various members that control the creation of the view

*poCallback*
:   Pointer to a class that implements [IEdmCardViewCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html)

#### Return Value

[IEdmCardView63](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView63.html)

# ![](dotnetimages/collapse.gif)Example

[Create Custom Card View (VB.NET)](Create_Custom_Card_View_Example_VBNET.htm)

[Create Custom Card View (C#)](Create_Custom_Card_View_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use this method if you want complete control of the loading and saving of data to and from a custom file or folder data card. Use [IEdmFolder5::CreateCardView](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateCardView.html) if you want SOLIDWORKS PDM Professional to handle the loading and saving of data to and from a simple file or folder data card.

This method supersedes [IEdmVault6::CreateCardViewEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6~CreateCardViewEx.html) by allowing you to pass a structure instead of individual parameters.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10.html)

[IEdmVault10 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009