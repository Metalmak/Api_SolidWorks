<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom~InsertRow.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| InsertRow Method (IEdmSWBom) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSWBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom.html) : InsertRow Method (IEdmSWBom) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lNr*
:   0-based index where to insert the row; 0 to insert in first position, -1 to insert at last position

Inserts a row at the specified index.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function InsertRow( _    ByVal lNr As System.Integer _ ) As EdmSWBomRow ``` | |

| C# |  |
| --- | --- |
| ``` EdmSWBomRow InsertRow(     System.int lNr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmSWBomRow^ InsertRow(  &   System.int lNr ) ``` | |

#### Parameters

*lNr*
:   0-based index where to insert the row; 0 to insert in first position, -1 to insert at last position

#### Return Value

[IEdmSWBomRow](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBomRow.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSWBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom.html)

[IEdmSWBom Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021 SP03