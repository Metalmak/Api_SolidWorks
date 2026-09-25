<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetColumnType3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetColumnType3 Method (ITableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : SetColumnType3 Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   0-based index of the column whose type to set

*ColumnType*
:   Type of column as defined in swTableColumnTypes\_e (see **Remarks**)

*IncludeHidden*
:   True to include hidden columns in Index, false to not

*PropertyData*
:   Property data specific to ColumnType (see **Remarks**)

Sets the type and property data for the specified BOM table column.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetColumnType3( _    ByVal Index As System.Integer, _    ByVal ColumnType As System.Integer, _    ByVal IncludeHidden As System.Boolean, _    ByVal PropertyData As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim Index As System.Integer Dim ColumnType As System.Integer Dim IncludeHidden As System.Boolean Dim PropertyData As System.Object Dim value As System.Integer   value = instance.SetColumnType3(Index, ColumnType, IncludeHidden, PropertyData) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetColumnType3(     System.int Index,    System.int ColumnType,    System.bool IncludeHidden,    System.object PropertyData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetColumnType3(  &   System.int Index, &   System.int ColumnType, &   System.bool IncludeHidden, &   System.Object^ PropertyData ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   0-based index of the column whose type to set

*ColumnType*
:   Type of column as defined in swTableColumnTypes\_e (see **Remarks**)

*IncludeHidden*
:   True to include hidden columns in Index, false to not

*PropertyData*
:   Property data specific to ColumnType (see **Remarks**)

#### Return Value

Return code as defined in swColumnTypeStatus\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::SetColumnType3.

# ![](dotnetimages/collapse.gif)Example

[Get and Set BOM Column Types and Cell Equations (VBA)](Get_and_Set_Column_Types_and_Cell_Equations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

PropertyData specifies the column title and contents.

| If ColumnType is set to swTableColumnTypes\_e.... | Then Set PropertyData with... |
| --- | --- |
| swBomTableColumnType\_CustomProperty | Valid property name\* |
| swBomTableColumnType\_UnitOfMeasure | Valid property name\* |
| swBomTableColumnType\_Equation | Equation string |
| swBomTableColumnType\_ComponentReference | Null or Nothing |
| swBomTableColumnType\_ToolboxProperty | Property as defined in swToolBoxPropertyName\_e |
| swBomTableColumnType\_CutListProperties (valid only for sheetmetal parts) | Valid cutlist property name\* |
| swBomTableColumnType\_ItemNumber | Array of four values {*Start\_Item\_Int*, *Increment\_Int*, *Order\_balloons\_and\_BOM\_to\_follow\_assembly\_order\_Bool*, *Do\_not\_change\_BOM\_item\_number\_Bool*} |
| swBomTableColumnType\_PartNumber | True to use title summary, false to not |

\* Note: To get the valid property names for a given column type, open a part in SOLIDWORKS and add a BOM table to it. Right-click a column and select **Insert > Column Right**. In the popup, select the column type of interest in the first dropdown. Inspect the contents of the second dropdown to see the valid property names for the column type.

When you set a column type, the title is automatically changed to match that column type. If you change the column type to custom property, you must set the column title using [ITableAnnotation::SetColumnTitle2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetColumnTitle2.html).

This method is consistent with the SOLIDWORKS user interface where you cannot add, delete, or replace the Quantity type column in a BOM table.

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::GetColumnType3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetColumnType3.html)

[ITableAnnotation::SetCellEquation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetCellEquation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0