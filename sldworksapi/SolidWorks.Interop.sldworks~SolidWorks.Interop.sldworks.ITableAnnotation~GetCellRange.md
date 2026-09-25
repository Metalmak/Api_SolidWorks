<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetCellRange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCellRange Method (ITableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : GetCellRange Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstRow*
:   Index of row of first selected cell

*LastRow*
:   Index of row of last selected cell

*FirstColumn*
:   Index of column of first selected cell

*LastColumn*
:   Index of column of last selected cell

Gets the selected table cells' row and column index ranges.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetCellRange( _    ByRef FirstRow As System.Integer, _    ByRef LastRow As System.Integer, _    ByRef FirstColumn As System.Integer, _    ByRef LastColumn As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim FirstRow As System.Integer Dim LastRow As System.Integer Dim FirstColumn As System.Integer Dim LastColumn As System.Integer   instance.GetCellRange(FirstRow, LastRow, FirstColumn, LastColumn) ``` | |

| C# |  |
| --- | --- |
| ``` void GetCellRange(     out System.int FirstRow,    out System.int LastRow,    out System.int FirstColumn,    out System.int LastColumn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetCellRange(  &   [Out] System.int FirstRow, &   [Out] System.int LastRow, &   [Out] System.int FirstColumn, &   [Out] System.int LastColumn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FirstRow*
:   Index of row of first selected cell

*LastRow*
:   Index of row of last selected cell

*FirstColumn*
:   Index of column of first selected cell

*LastColumn*
:   Index of column of last selected cell

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::GetCellRange.

# ![](dotnetimages/collapse.gif)Example

[Select Table Cells (C#)](Select_Table_Cells_Example_CSharp.htm)

[Select Table Cells (VB.NET)](Select_Table_Cells_Example_VBNET.htm)

[Select Table Cells (VBA)](Select_Table_Cells_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The returned indexes are all 0-based.

If you don't multi-select table cells before you call this method, then the cell row/column index range for the entire table is returned.

Before calling this method, you can select the table cells in the graphics area whose row/column index range you want to get. How you make these selections determines what this method returns.

|  |  |  |
| --- | --- | --- |
| **Selection** | **Steps** | **Cell range returned** |
| Table cell | 1. Place the cursor on the desired table cell.- Click the left-mouse button. | Selected cell |
|  | 1. Hold down the Ctrl key and place the cursor on the desired table cell.- Click the left-mouse button. | Selected cell |
| Multiple table cells | 1. Place the cursor on a desired table cell.- Click and hold down the left-mouse button.- Drag the cursor over the other desired table cells.- Release the left-mouse button when the cursor is on the last table cell that you want selected. | All selected cells |
|  | 1. Hold down the Ctrl key and place the cursor on a desired table cell.- Click the left-mouse button.- Repeat steps 1 and 2 until all desired table cells are selected. | Each selected cell |
| Table column | Place the cursor just above the desired column and click the left-mouse button when the cursor changes to a solid arrow | All selected cells |
| Table row | Place the cursor to just left of the desired row and click the left-mouse button when the cursor changes to a solid arrow | All selected cells |

Run any of the examples in the **Example** section to better understand the values returned by this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::GetCellTextFormat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetCellTextFormat.html)

[ITableAnnotation::GetCellUseDocTextFormat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetCellUseDocTextFormat.html)

[ITableAnnotation::IsCellMerged Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~IsCellMerged.html)

[ITableAnnotation::IsCellTextEditable Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~IsCellTextEditable.html)

[ITableAnnotation::MergeCells Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~MergeCells.html)

[ITableAnnotation::SetCellRange Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetCellRange.html)

[ITableAnnotation::SetCellTextFormat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetCellTextFormat.html)

[ITableAnnotation::CellTextHorizontalJustification Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~CellTextHorizontalJustification.html)

[ITableAnnotation::CellTextVerticalJustification Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~CellTextVerticalJustification.html)

[ITableAnnotation::DisplayedText Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~DisplayedText.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0