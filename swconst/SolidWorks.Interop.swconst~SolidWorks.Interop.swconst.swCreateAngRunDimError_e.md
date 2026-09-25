<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCreateAngRunDimError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCreateAngRunDimError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCreateAngRunDimError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Statuses when inserting an angular running dimension.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCreateAngRunDimError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCreateAngRunDimError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCreateAngRunDimError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCreateAngRunDimError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCreateAngRunDimError\_GenFailure** | 0 = Cannot create this angular running dimension |
| **swCreateAngRunDimError\_IdenticalDimension** | 2 = Identical dimensions cannot be created in the same angular running dimension |
| **swCreateAngRunDimError\_SelectAnotherEntity** | 3 = Cannot use the selected entity to create this angular running dimension; select another entity |
| **swCreateAngRunDimError\_Success** | 1 |
| **swCreateAngRunDimError\_Undefined** | -1 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)