<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData~Ascending.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Ascending Property (IBomTableSortData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableSortData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html) : Ascending Property (IBomTableSortData) |

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

Gets and sets whether this is an ascending sort for the specified sort order index.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Ascending( _    ByVal SortOrderIndex As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableSortData Dim SortOrderIndex As System.Integer Dim value As System.Boolean   instance.Ascending(SortOrderIndex) = value   value = instance.Ascending(SortOrderIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Ascending(     System.int SortOrderIndex ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool Ascending {    System.bool get(System.int SortOrderIndex);    void set (System.int SortOrderIndex, System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SortOrderIndex*
:   0 for primary sort, 1 for secondary sort, 2 for tertiary sort (see **Remarks**)

#### Property Value

True if sort is ascending, false if descending

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomTableSortData::Ascending.

# ![](dotnetimages/collapse.gif)Example

See the [IBomTableSortData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

BOM tables may be sorted by up to three columns. This property maps the sort order index with a sorting direction (ascending or descending). Call this property three times to set the sorting directions of all three sort order indexes.

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableSortData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html)

[IBomTableSortData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0