<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralTableAnnotation~Sort.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Sort Method (IGeneralTableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGeneralTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralTableAnnotation.html) : Sort Method (IGeneralTableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ColumnIndex*
:   0-based index of column to sort by

*SortAscending*
:   True to sort ascending, false to sort descending

Sorts this table by the specified column in the specified sorting direction.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Sort( _    ByVal ColumnIndex As System.Integer, _    ByVal SortAscending As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGeneralTableAnnotation Dim ColumnIndex As System.Integer Dim SortAscending As System.Boolean Dim value As System.Boolean   value = instance.Sort(ColumnIndex, SortAscending) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Sort(     System.int ColumnIndex,    System.bool SortAscending ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Sort(  &   System.int ColumnIndex, &   System.bool SortAscending ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ColumnIndex*
:   0-based index of column to sort by

*SortAscending*
:   True to sort ascending, false to sort descending

#### Return Value

True if sorted successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See GeneralTableAnnotation::Sort.

# ![](dotnetimages/collapse.gif)Example

[Sort Table (VBA)](Sort_Table_Example_VB.htm)

[Sort Table (VB.NET)](Sort_Table_Example_VBNET.htm)

[Sort Table (C#)](Sort_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

See Sorting Tables for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[IGeneralTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralTableAnnotation.html)

[IGeneralTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralTableAnnotation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0