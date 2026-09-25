<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView5~GetCardSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCardSize Method (IEdmCardView5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardView5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView5.html) : GetCardSize Method (IEdmCardView5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*plWidth*
:   Width of the card in pixels

*plHeight*
:   Height of the card in pixels

Gets the size of the file or folder data card.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetCardSize( _    ByRef plWidth As System.Integer, _    ByRef plHeight As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetCardSize(     out System.int plWidth,    out System.int plHeight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetCardSize(  &   [Out] System.int plWidth, &   [Out] System.int plHeight ) ``` | |

#### Parameters

*plWidth*
:   Width of the card in pixels

*plHeight*
:   Height of the card in pixels

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardView5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardView5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView5.html)

[IEdmCardView5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2