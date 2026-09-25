<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetCellTextOrientation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetCellTextOrientation Method (ITableAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : SetCellTextOrientation Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Row*
:   0-based index of row; valid only if AllCells is set to false

*Column*
:   0-based index of column; valid only if AllCells is set to false

*IncludeHidden*
:   True to include hidden rows and columns in the Row and Column indexes, false to not

*AllCells*
:   True for all cells, false if not; if false, set Row and Column

*Orientation*
:   Text orientation as defined in swTableCellOrientation\_e (see **Remarks**)

Sets the text orientation in the specified table cell.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetCellTextOrientation( _    ByVal Row As System.Integer, _    ByVal Column As System.Integer, _    ByVal IncludeHidden As System.Boolean, _    ByVal AllCells As System.Boolean, _    ByVal Orientation As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim Row As System.Integer Dim Column As System.Integer Dim IncludeHidden As System.Boolean Dim AllCells As System.Boolean Dim Orientation As System.Integer   instance.SetCellTextOrientation(Row, Column, IncludeHidden, AllCells, Orientation) ``` | |

| C# |  |
| --- | --- |
| ``` void SetCellTextOrientation(     System.int Row,    System.int Column,    System.bool IncludeHidden,    System.bool AllCells,    System.int Orientation ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetCellTextOrientation(  &   System.int Row, &   System.int Column, &   System.bool IncludeHidden, &   System.bool AllCells, &   System.int Orientation ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Row*
:   0-based index of row; valid only if AllCells is set to false

*Column*
:   0-based index of column; valid only if AllCells is set to false

*IncludeHidden*
:   True to include hidden rows and columns in the Row and Column indexes, false to not

*AllCells*
:   True for all cells, false if not; if false, set Row and Column

*Orientation*
:   Text orientation as defined in swTableCellOrientation\_e (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::SetCellTextOrientation.

# ![](dotnetimages/collapse.gif)Remarks

You can set Orientation to any member of swTableCellOrientation\_e except swTableCellOrientation\_Varies.

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::GetCellTextOrientation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetCellTextOrientation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0