<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr~GetBomLayouts.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetBomLayouts Method (IEdmBomMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr.html) : GetBomLayouts Method (IEdmBomMgr) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetLayouts*
:   Array of [EdmBomLayout](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout.html) structures; one structure for each BOM layout

Obsolete. Superseded by [IEdmBomMgr2::GetBomLayouts2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2~GetBomLayouts2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetBomLayouts( _    ByRef ppoRetLayouts() As EdmBomLayout _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetBomLayouts(     out EdmBomLayout[] ppoRetLayouts ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetBomLayouts(  &   [Out] array<EdmBomLayout>^ ppoRetLayouts ) ``` | |

#### Parameters

*ppoRetLayouts*
:   Array of [EdmBomLayout](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout.html) structures; one structure for each BOM layout

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr.html)

[IEdmBomMgr Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009