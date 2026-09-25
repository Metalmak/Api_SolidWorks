<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swConfigTreeSortType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swConfigTreeSortType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swConfigTreeSortType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Order in which configurations are listed in the ConfigurationManager.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swConfigTreeSortType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swConfigTreeSortType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swConfigTreeSortType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swConfigTreeSortType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSortType\_DesignTable** | 3 = Order of the configurations in the ConfigurationManager is dictated by the order of the configurations in the design table |
| **swSortType\_History** | 0 = Order of the configurations in the ConfigurationManager is dictated by the date the configuration was created, from earliest created at the top of the list to most recently created at the bottom of the list |
| **swSortType\_Literal** | 2 = Order of the configurations in the ConfigurationManager is alphabetical |
| **swSortType\_Numeric** | 1 = Order of the configurations in the ConfigurationManager is by ascending alpha or numeric value |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)