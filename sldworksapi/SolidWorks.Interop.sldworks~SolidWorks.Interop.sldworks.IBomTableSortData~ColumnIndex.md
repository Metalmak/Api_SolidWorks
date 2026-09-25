<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData~ColumnIndex.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ColumnIndex Property (IBomTableSortData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableSortData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html) : ColumnIndex Property (IBomTableSortData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SortOrderIndex*
:   0 for primary sort, 1 for secondary sort, 2 for tertiary sort (see **Remarks**)

Gets and sets the column index for the specified sort order index.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ColumnIndex( _    ByVal SortOrderIndex As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableSortData Dim SortOrderIndex As System.Integer Dim value As System.Integer   instance.ColumnIndex(SortOrderIndex) = value   value = instance.ColumnIndex(SortOrderIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ColumnIndex(     System.int SortOrderIndex ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ColumnIndex {    System.int get(System.int SortOrderIndex);    void set (System.int SortOrderIndex, System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SortOrderIndex*
:   0 for primary sort, 1 for secondary sort, 2 for tertiary sort (see **Remarks**)

#### Property Value

0-based column index mapped to the specified SortOrderIndex; specify -1 if the specified SortOrderIndex is not used

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomTableSortData::ColumnIndex.

# ![](dotnetimages/collapse.gif)Example

See the [IBomTableSortData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

BOM tables may be sorted by up to three columns. This property maps one column to a sort order index. Call this property three times to set the sort order indexes of all three columns.

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableSortData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html)

[IBomTableSortData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0