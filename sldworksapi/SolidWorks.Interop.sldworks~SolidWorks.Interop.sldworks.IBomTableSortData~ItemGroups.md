<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData~ItemGroups.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ItemGroups Property (IBomTableSortData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableSortData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html) : ItemGroups Property (IBomTableSortData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the categories into which the BOM table rows are grouped.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ItemGroups As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableSortData Dim value As System.Object   instance.ItemGroups = value   value = instance.ItemGroups ``` | |

| C# |  |
| --- | --- |
| ``` System.object ItemGroups {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ ItemGroups {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array of categories as defined in swBomTableSortItemGroup\_e or null (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomTableSortData::ItemGroups.

# ![](dotnetimages/collapse.gif)Example

See the [IBomTableSortData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

You can set this property in one of two ways:

* Specify null to indicate that the BOM table rows are not to be grouped into categories.* Specify an array of three swBomTableSortItemGroup\_e enumerators to indicate that the BOM table rows are to be grouped into three categories (assemblies, parts, other).

For example, when you set this property to an array of three enumerators in the following order, assemblies are grouped first, parts are grouped next, and other categories are grouped last:

1. swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_Assemblies- swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_Parts- swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_Other

Substitute any enumerator in the array with swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_None to eliminate grouping into that category.

For example, when you set this property to the following array, no assemblies are grouped, parts are grouped first, and other categories are grouped last:

1. swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_None- swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_Parts- swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_Other

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableSortData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html)

[IBomTableSortData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0