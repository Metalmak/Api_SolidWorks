<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetCSVersionDialog~Show.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Show Method (IEdmGetCSVersionDialog) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmGetCSVersionDialog Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetCSVersionDialog.html) : Show Method (IEdmGetCSVersionDialog) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*peReply*
:   [EdmGetOpReply](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetOpReply.html); user-defined action

*vbApplyForAll*
:   True to apply peReply to all items, false to not

Shows the Restore coldstored file version dialog.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Show( _    ByRef peReply As EdmGetOpReply, _    ByRef vbApplyForAll As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Show(     out EdmGetOpReply peReply,    out System.bool vbApplyForAll ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Show(  &   [Out] EdmGetOpReply peReply, &   [Out] System.bool vbApplyForAll ) ``` | |

#### Parameters

*peReply*
:   [EdmGetOpReply](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetOpReply.html); user-defined action

*vbApplyForAll*
:   True to apply peReply to all items, false to not

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmGetCSVersionDialog Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetCSVersionDialog.html)

[IEdmGetCSVersionDialog Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetCSVersionDialog_members.html)