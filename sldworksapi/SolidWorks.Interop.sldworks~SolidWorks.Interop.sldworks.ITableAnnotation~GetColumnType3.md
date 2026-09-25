<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetColumnType3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetColumnType3 Method (ITableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : GetColumnType3 Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   0-based index of the column whose type to get

*IncludeHidden*
:   True to include hidden columns in Index, false to not

*PropertyData*
:   Property data specific to the type of column (see **Remarks**)

*Status*
:   Return code as defined in swColumnTypeStatus\_e

Gets the type and property data for the specified BOM table column.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetColumnType3( _    ByVal Index As System.Integer, _    ByVal IncludeHidden As System.Boolean, _    ByRef PropertyData As System.Object, _    ByRef Status As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim Index As System.Integer Dim IncludeHidden As System.Boolean Dim PropertyData As System.Object Dim Status As System.Integer Dim value As System.Integer   value = instance.GetColumnType3(Index, IncludeHidden, PropertyData, Status) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetColumnType3(     System.int Index,    System.bool IncludeHidden,    out System.object PropertyData,    out System.int Status ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetColumnType3(  &   System.int Index, &   System.bool IncludeHidden, &   [Out] System.Object^ PropertyData, &   [Out] System.int Status ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   0-based index of the column whose type to get

*IncludeHidden*
:   True to include hidden columns in Index, false to not

*PropertyData*
:   Property data specific to the type of column (see **Remarks**)

*Status*
:   Return code as defined in swColumnTypeStatus\_e

#### Return Value

Type of column as defined in swTableColumnTypes\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::GetColumnType3.

# ![](dotnetimages/collapse.gif)Example

[Get and Set BOM Column Types and Cell Equations (VBA)](Get_and_Set_Column_Types_and_Cell_Equations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

PropertyData varies by the type of column. See the Remarks in [ITableAnnotation::SetColumnType3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetColumnType3.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::GetCellEquation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetCellEquation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0