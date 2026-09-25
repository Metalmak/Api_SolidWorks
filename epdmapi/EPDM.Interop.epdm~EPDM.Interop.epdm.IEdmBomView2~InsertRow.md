<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView2~InsertRow.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| InsertRow Method (IEdmBomView2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomView2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView2.html) : InsertRow Method (IEdmBomView2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poRow*
:   [IEdmBomCell](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html); existing row

*eInsertOption*
:   Where the new BOM row is inserted with respect to poRow as defined in [EdmBomInsertRowOption](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInsertRowOption.html)

*ppoNewRow*
:   [IEdmBomCell](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html)

Inserts a row into this named BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub InsertRow( _    ByVal poRow As EdmBomCell, _    ByVal eInsertOption As EdmBomInsertRowOption, _    ByRef ppoNewRow As EdmBomCell _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertRow(     EdmBomCell poRow,    EdmBomInsertRowOption eInsertOption,    out EdmBomCell ppoNewRow ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertRow(  &   EdmBomCell^ poRow, &   EdmBomInsertRowOption eInsertOption, &   [Out] EdmBomCell^ ppoNewRow ) ``` | |

#### Parameters

*poRow*
:   [IEdmBomCell](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html); existing row

*eInsertOption*
:   Where the new BOM row is inserted with respect to poRow as defined in [EdmBomInsertRowOption](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInsertRowOption.html)

*ppoNewRow*
:   [IEdmBomCell](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html)

# ![](dotnetimages/collapse.gif)Example

[Add Row to Bill of Materials (VB.NET)](Add_Row_to_Bill_of_Materials_Example_VBNET.htm)

[Add Row to Bill of Materials (C#)](Add_Row_to_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for named BOMs.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomView2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView2.html)

[IEdmBomView2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011 SP04