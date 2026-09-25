<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAddMateError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAddMateError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAddMateError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Status after adding or editing a mate.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAddMateError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAddMateError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAddMateError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAddMateError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAddMateError\_ErrorUknown** | 0 = Unknown error occurred |
| **swAddMateError\_IncorrectAlignment** | 3 = Unknown mate alignment or mate alignment is not present in [swMateAlign\_e](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swMateAlign_e.html) |
| **swAddMateError\_IncorrectGearRatios** | 6 = Mate gear ratios are invalid |
| **swAddMateError\_IncorrectMateType** | 2 = Unknown mate type or mate type not present in [swMateType\_e](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swMateType_e.html) |
| **swAddMateError\_IncorrectSelections** | 4 = Incorrect selections for mate |
| **swAddMateError\_NoError** | 1 = Success, no error |
| **swAddMateError\_OverDefinedAssembly** | 5 = Mate is over-defining the assembly |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)