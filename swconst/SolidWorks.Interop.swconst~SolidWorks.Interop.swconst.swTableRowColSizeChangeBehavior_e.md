<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swTableRowColSizeChangeBehavior_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swTableRowColSizeChangeBehavior\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swTableRowColSizeChangeBehavior\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Values indicate how the size of the rest of the table should behave when a height of a row or width of a column changes.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swTableRowColSizeChangeBehavior_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swTableRowColSizeChangeBehavior_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swTableRowColSizeChangeBehavior_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swTableRowColSizeChangeBehavior_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swTableRowColChange\_AbsorbedByNext** | 1 = The next row or column must absorb the change in size so that the entire table size remains the same |
| **swTableRowColChange\_AbsorbedByPrevious** | 2 = The next row or column must absorb the change in size so that the entire table size remains the same |
| **swTableRowColChange\_TableSizeCanChange** | 0 = The remaining rows or columns can shift, so that the entire table width or height changes |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)