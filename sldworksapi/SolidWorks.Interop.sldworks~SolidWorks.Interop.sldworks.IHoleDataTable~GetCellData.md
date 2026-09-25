<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleDataTable~GetCellData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCellData Method (IHoleDataTable) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleDataTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleDataTable.html) : GetCellData Method (IHoleDataTable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ColumnName*
:   Column name (see **Remarks**)

*RowIndex*
:   0-based row index

*CellData*
:   Cell data

Gets data from the specified table cell of this Hole Wizard fastener table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCellData( _    ByVal ColumnName As System.String, _    ByVal RowIndex As System.Integer, _    ByRef CellData As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleDataTable Dim ColumnName As System.String Dim RowIndex As System.Integer Dim CellData As System.String Dim value As System.Boolean   value = instance.GetCellData(ColumnName, RowIndex, CellData) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetCellData(     System.string ColumnName,    System.int RowIndex,    out System.string CellData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetCellData(  &   System.String^ ColumnName, &   System.int RowIndex, &   [Out] System.String^ CellData ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ColumnName*
:   Column name (see **Remarks**)

*RowIndex*
:   0-based row index

*CellData*
:   Cell data

#### Return Value

True if cell data successfully retrieved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HoleDataTable::GetCellData.

# ![](dotnetimages/collapse.gif)Example

See the [IHoleDataTable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleDataTable.html) example.

# ![](dotnetimages/collapse.gif)Remarks

To set:

* ColumnName, use [IHoleDataTable::GetColumnNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleDataTable~GetColumnNames.html).* RowIndex, use [IHoleDataTable::GetRowCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleDataTable~GetRowCount.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleDataTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleDataTable.html)

[IHoleDataTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleDataTable_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0