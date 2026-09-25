<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSMBendState_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSMBendState\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSMBendState\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Bend state values for a sheet metal part.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSMBendState_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSMBendState_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSMBendState_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSMBendState_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSMBendStateFlattened** | 2 = The bends are flattened; the model is rolled back to just after a FlattenBends feature, but just before the corresponding ProcessBends feature |
| **swSMBendStateFolded** | 3 = The bends are folded; the model is rolled back to just after a FlattenBends ProcessBends feature pair |
| **swSMBendStateNone** | 0 = Not a sheet metal part; no SheetMetal features present |
| **swSMBendStateSharps** | 1 = The bends are in their sharp state; the part is rolled back to just before the first FlattenBends feature |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)