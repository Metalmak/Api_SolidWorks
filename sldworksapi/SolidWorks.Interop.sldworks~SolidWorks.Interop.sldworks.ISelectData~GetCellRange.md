<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectData~GetCellRange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCellRange Method (ISelectData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISelectData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectData.html) : GetCellRange Method (ISelectData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstRow*
:   0-based row number at the beginning of the selection range

*LastRow*
:   0-based row number at the end of the selection range

*FirstColumn*
:   0-based column number at the beginning of the selection range

*LastColumn*
:   0-based column number at the end of the selection range

Gets the specified range of table cells for this selection.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetCellRange( _    ByRef FirstRow As System.Integer, _    ByRef LastRow As System.Integer, _    ByRef FirstColumn As System.Integer, _    ByRef LastColumn As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISelectData Dim FirstRow As System.Integer Dim LastRow As System.Integer Dim FirstColumn As System.Integer Dim LastColumn As System.Integer   instance.GetCellRange(FirstRow, LastRow, FirstColumn, LastColumn) ``` | |

| C# |  |
| --- | --- |
| ``` void GetCellRange(     out System.int FirstRow,    out System.int LastRow,    out System.int FirstColumn,    out System.int LastColumn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetCellRange(  &   [Out] System.int FirstRow, &   [Out] System.int LastRow, &   [Out] System.int FirstColumn, &   [Out] System.int LastColumn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FirstRow*
:   0-based row number at the beginning of the selection range

*LastRow*
:   0-based row number at the end of the selection range

*FirstColumn*
:   0-based column number at the beginning of the selection range

*LastColumn*
:   0-based column number at the end of the selection range

#### Return Value

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SelectData::GetCellRange.

# ![](dotnetimages/collapse.gif)Remarks

The range of table cells are only used for a selection made in a table. For all other types of selections, these values are ignored.

By default, the value for FirstRow, LastRow, FirstColumn, and LastColumn is -1, which indicates that the entire table is selected.

# ![](dotnetimages/collapse.gif)See Also

####

[ISelectData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectData.html)

[ISelectData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectData_members.html)

[ISelectData::SetCellRange Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectData~SetCellRange.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0