<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swBomTableSortItemGroup_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swBomTableSortItemGroup\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swBomTableSortItemGroup\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Categories for sorting bill of material table rows.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swBomTableSortItemGroup_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swBomTableSortItemGroup_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swBomTableSortItemGroup_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swBomTableSortItemGroup_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swBomTableSortItemGroup\_Assemblies** | 1 = Group table rows containing assemblies |
| **swBomTableSortItemGroup\_None** | 0 = No groupings (see **Remarks**) |
| **swBomTableSortItemGroup\_Other** | 4 = Group table rows containing user-defined items |
| **swBomTableSortItemGroup\_Parts** | 2 = Group table rows containing parts |

# ![](dotnetimages/collapse.gif)Remarks

These enumerator options are used by IBomTableSortData::ItemGroups to set the groupings for table sorting. Use swBomTableSortItemGroup\_None instead of one or more of the other options to indicate which groupings the sort will not perform.

For example, when you set IBomTableSortData::ItemGroups to the following array, no assemblies are grouped, parts are grouped first, and other categories are grouped last:

1. swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_None- swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_Parts- swBomTableSortItemGroup\_e.swBomTableSortItemGroup\_Other

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)