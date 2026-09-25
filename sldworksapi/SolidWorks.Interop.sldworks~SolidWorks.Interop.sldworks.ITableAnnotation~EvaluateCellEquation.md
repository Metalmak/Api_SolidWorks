<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~EvaluateCellEquation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EvaluateCellEquation Method (ITableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : EvaluateCellEquation Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Row*
:   0-based index of the row

*Column*
:   0-based index of the column

*IncludeHidden*
:   True to include hidden rows and columns in the Row and Column indexes, false to not

*Equation*
:   Equation to solve; empty string to remove an equation

*SolvedValue*
:   Value of solved Equation

Solves the specified equation in the specified cell of this BOM table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EvaluateCellEquation( _    ByVal Row As System.Integer, _    ByVal Column As System.Integer, _    ByVal IncludeHidden As System.Boolean, _    ByVal Equation As System.String, _    ByRef SolvedValue As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim Row As System.Integer Dim Column As System.Integer Dim IncludeHidden As System.Boolean Dim Equation As System.String Dim SolvedValue As System.String Dim value As System.Integer   value = instance.EvaluateCellEquation(Row, Column, IncludeHidden, Equation, SolvedValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int EvaluateCellEquation(     System.int Row,    System.int Column,    System.bool IncludeHidden,    System.string Equation,    out System.string SolvedValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int EvaluateCellEquation(  &   System.int Row, &   System.int Column, &   System.bool IncludeHidden, &   System.String^ Equation, &   [Out] System.String^ SolvedValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Row*
:   0-based index of the row

*Column*
:   0-based index of the column

*IncludeHidden*
:   True to include hidden rows and columns in the Row and Column indexes, false to not

*Equation*
:   Equation to solve; empty string to remove an equation

*SolvedValue*
:   Value of solved Equation

#### Return Value

Return code as defined in swCellEquationStatus\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::EvaluateCellEquation.

# ![](dotnetimages/collapse.gif)Example

[Get and Set BOM Column Types and Cell Equations (VBA)](Get_and_Set_Column_Types_and_Cell_Equations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::GetCellEquation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetCellEquation.html)

[ITableAnnotation::SetCellEquation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetCellEquation.html)

[ITableAnnotation::GetColumnType3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetColumnType3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0