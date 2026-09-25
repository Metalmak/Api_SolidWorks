<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetRowHeight.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetRowHeight Method (ITableAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : SetRowHeight Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index of row for which to set height

*Height*
:   Height at which to set specified row, in system units

*Options*
:   Table's behavior after changing row as defined by swTableRowColSizeChangeBehavior\_e (see **Remarks**)

Sets the height of the specified row in this table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetRowHeight( _    ByVal Index As System.Integer, _    ByVal Height As System.Double, _    ByVal Options As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim Index As System.Integer Dim Height As System.Double Dim Options As System.Integer Dim value As System.Double   value = instance.SetRowHeight(Index, Height, Options) ``` | |

| C# |  |
| --- | --- |
| ``` System.double SetRowHeight(     System.int Index,    System.double Height,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double SetRowHeight(  &   System.int Index, &   System.double Height, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Index of row for which to set height

*Height*
:   Height at which to set specified row, in system units

*Options*
:   Table's behavior after changing row as defined by swTableRowColSizeChangeBehavior\_e (see **Remarks**)

#### Return Value

Height to which specified row is set (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::SetRowHeight.

# ![](dotnetimages/collapse.gif)Remarks

The index for both rows and columns is 0-based.

Index is the number of the row whose height to set. The first row is row 0.  It can also be a value from the swTableCellRangeIdentifier\_e enumerator.

| **If Index equals...** | **Then the height of all of the rows...** |
| --- | --- |
| swTableCellRange\_All | Is set, if possible. |
| swTableCellRange\_Current | In the current range (see [ITableAnnotation::GetCellRange](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~GetCellRange.html) and [ITableAnnotation::SetCellRange](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~SetCellRange.html)) is set, if possible |

When the height of a row changes, then the rest of the table is affected. The Options argument indicates the rest of the table's behavior.

|  |  |
| --- | --- |
| **If...** | **Then...** |
| Options = swTableRowColChange\_TableSizeCanChange | The rest of the rows remain the same height and are shifted away from the table anchor to make room for the changed row. |
| Height of the entire table must remain the same, so that the table continues to fit properly on the drawing | Other rows must absorb the change in height. There are two possibilities supported by this method.   * If Options = swTableRowColChange\_AbsorbedByNext, then first row below the rows whose height has changed, are adjusted if possible.  If that is not possible, then the first row above the rows whose height has changed, is adjusted if possible. If that is not possible either, then no action is taken.   * The other similar case is if Options = swTableRowColChange\_AbsorbedByPrevious. First the row above is tried, then the row below. |
| Options = swTableRowColChange\_AbsorbedByNext or swTableRowColChange\_AbsorbedByPrevious | It might not be possible to get the desired results. If this is the case, then you must determine the full height of the table yourself and set row heights individually using the swTableRowColChange\_TableSizeCanChange option, making sure to end up with the original  table height. |

The return value is the height at which the row is set. If you specified a range of rows, it is the height of the first row of that range.

It is possible that the return value is different than the value that you passed in. One possibility is that if you specify a row height that is less than the minimum row height, then the minimum row height is used instead of what you specified. Another possibility is that if you are trying to maintain a fixed table height, but the height of the adjacent rows is not big enough to absorb the height changes to the rows that you specified, then the return value is the same as the row's original width instead of what you specified.

To get the row height, use [ITableAnnotation::GetRowHeight](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~GetCellRange.html).

To get or set the column width, use [ITableAnnotation::GetColumnWidth](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~GetColumnWidth.html) and [ITableAnnotation::SetColumnWidth](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~SetColumnWidth.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::DeleteRow Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~DeleteRow.html)

[ITableAnnotation::GetRowVerticalGap Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetRowVerticalGap.html)

[ITableAnnotation::InsertRow Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~InsertRow.html)

[ITableAnnotation::MoveRow Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~MoveRow.html)

[ITableAnnotation::SetRowVerticalGap Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetRowVerticalGap.html)

[ITableAnnotation::RowCount Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~RowCount.html)

[ITableAnnotation::TotalRowCount Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~TotalRowCount.html)

[ITableAnnotation::RowHidden Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~RowHidden.html)

[ITableAnnotation::GetLockRowHeight Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetLockRowHeight.html)

[ITableAnnotation::SetLockRowHeight Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetLockRowHeight.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0