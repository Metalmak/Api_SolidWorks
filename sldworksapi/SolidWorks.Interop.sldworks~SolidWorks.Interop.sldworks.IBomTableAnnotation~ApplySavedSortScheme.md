<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~ApplySavedSortScheme.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ApplySavedSortScheme Method (IBomTableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html) : ApplySavedSortScheme Method (IBomTableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SortData*
:   [IBomTableSortData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableSortData.html)

Sorts this BOM table using the sort data that was previously saved in the table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ApplySavedSortScheme( _    ByVal SortData As BomTableSortData _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableAnnotation Dim SortData As BomTableSortData Dim value As System.Boolean   value = instance.ApplySavedSortScheme(SortData) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ApplySavedSortScheme(     BomTableSortData SortData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ApplySavedSortScheme(  &   BomTableSortData^ SortData ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SortData*
:   [IBomTableSortData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableSortData.html)

#### Return Value

True if BOM table is successfully sorted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomTableAnnotation::ApplySavedSortScheme.

# ![](dotnetimages/collapse.gif)Example

[Sort Table (VBA)](Sort_Table_Example_VB.htm)

[Sort Table (VB.NET)](Sort_Table_Example_VBNET.htm)

[Sort Table (C#)](Sort_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must:

1. Set [IBomTableSortData::SaveCurrentSortParameters](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableSortData~SaveCurrentSortParameters.html) to true to indicate that the sort settings should be saved in the BOM table in the drawing.- [IBomTableAnnotation::Sort](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation~Sort.html) to actually save the sort settings in the BOM table in the drawing.- [IBomTableAnnotation::GetBomTableSortData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation~GetBomTableSortData.html) to populate SortData.

See Sorting Tables for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html)

[IBomTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0