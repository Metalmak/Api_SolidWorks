<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom~InsertColumn.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| InsertColumn Method (IEdmSWBom) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSWBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom.html) : InsertColumn Method (IEdmSWBom) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lNr*
:   0-based index where to insert the column; 0 to insert column in first position, -1 to insert column in last position

*pbsName*
:   Name of column

Inserts a column at the specified column index.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function InsertColumn( _    ByVal lNr As System.Integer, _    ByVal pbsName As System.String _ ) As EdmSWBomColumn ``` | |

| C# |  |
| --- | --- |
| ``` EdmSWBomColumn InsertColumn(     System.int lNr,    System.string pbsName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmSWBomColumn^ InsertColumn(  &   System.int lNr, &   System.String^ pbsName ) ``` | |

#### Parameters

*lNr*
:   0-based index where to insert the column; 0 to insert column in first position, -1 to insert column in last position

*pbsName*
:   Name of column

#### Return Value

[IEdmSWBomColumn](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBomColumn.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSWBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom.html)

[IEdmSWBom Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021 SP03