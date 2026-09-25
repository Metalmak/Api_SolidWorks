<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom~GetCell.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCell Method (IEdmSWBom) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSWBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom.html) : GetCell Method (IEdmSWBom) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lRowNr*
:   0-based index of cell row

*lColumnNr*
:   0-based index of cell column

Gets the specified cell in this BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetCell( _    ByVal lRowNr As System.Integer, _    ByVal lColumnNr As System.Integer _ ) As EdmSWBomCell ``` | |

| C# |  |
| --- | --- |
| ``` EdmSWBomCell GetCell(     System.int lRowNr,    System.int lColumnNr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmSWBomCell^ GetCell(  &   System.int lRowNr, &   System.int lColumnNr ) ``` | |

#### Parameters

*lRowNr*
:   0-based index of cell row

*lColumnNr*
:   0-based index of cell column

#### Return Value

[IEdmSWBomCell](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBomCell.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomMgr3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSWBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom.html)

[IEdmSWBom Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021 SP03