<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2~GetBomLayouts2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetBomLayouts2 Method (IEdmBomMgr2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2.html) : GetBomLayouts2 Method (IEdmBomMgr2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetLayouts*
:   Array of [EdmBomLayout2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout2.html) structures; one structure for each BOM layout

Gets all of the BOM layouts installed in a vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetBomLayouts2( _    ByRef ppoRetLayouts() As EdmBomLayout2 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetBomLayouts2(     out EdmBomLayout2[] ppoRetLayouts ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetBomLayouts2(  &   [Out] array<EdmBomLayout2>^ ppoRetLayouts ) ``` | |

#### Parameters

*ppoRetLayouts*
:   Array of [EdmBomLayout2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout2.html) structures; one structure for each BOM layout

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomMgr2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2.html)

[IEdmBomMgr2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2020