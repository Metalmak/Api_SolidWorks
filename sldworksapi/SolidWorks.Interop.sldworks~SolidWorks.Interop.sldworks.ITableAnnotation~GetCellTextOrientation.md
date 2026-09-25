<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetCellTextOrientation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCellTextOrientation Method (ITableAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : GetCellTextOrientation Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Row*
:   0-based index of the cell row; valid only if AllCells is set to false

*Column*
:   0-based index of the cell column; valid only if AllCells is set to false

*IncludeHidden*
:   True to include hidden rows and columns in Row and Column indexes, false to not

*AllCells*
:   True to get the orientation in all cells, false to not; if false, set Row and Column (see **Remarks**)

Gets the text orientation in the specified cell of this table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCellTextOrientation( _    ByVal Row As System.Integer, _    ByVal Column As System.Integer, _    ByVal IncludeHidden As System.Boolean, _    ByVal AllCells As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim Row As System.Integer Dim Column As System.Integer Dim IncludeHidden As System.Boolean Dim AllCells As System.Boolean Dim value As System.Integer   value = instance.GetCellTextOrientation(Row, Column, IncludeHidden, AllCells) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetCellTextOrientation(     System.int Row,    System.int Column,    System.bool IncludeHidden,    System.bool AllCells ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetCellTextOrientation(  &   System.int Row, &   System.int Column, &   System.bool IncludeHidden, &   System.bool AllCells ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Row*
:   0-based index of the cell row; valid only if AllCells is set to false

*Column*
:   0-based index of the cell column; valid only if AllCells is set to false

*IncludeHidden*
:   True to include hidden rows and columns in Row and Column indexes, false to not

*AllCells*
:   True to get the orientation in all cells, false to not; if false, set Row and Column (see **Remarks**)

#### Return Value

Text orientation as defined in swTableCellOrientation\_e (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::GetCellTextOrientation.

# ![](dotnetimages/collapse.gif)Remarks

If AllCells is set to false, this method returns one of swTableCellOrientation\_e.:

* swTableCellOrientation\_Right* swTableCellOrientation\_Left* swTableCellOrientation\_Up* swTableCellOrientation\_Down

If AllCells is set to true, this method returns one of the above or:

* swTableCellOrientation\_Varies, if all the cells do not share the same text orientation.

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::SetCellTextOrientation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetCellTextOrientation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0