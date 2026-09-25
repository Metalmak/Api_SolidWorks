<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swReverseEndPointTangentResult_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swReverseEndPointTangentResult\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swReverseEndPointTangentResult\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Result codes for ISketchManager::ReverseEndPointTangent.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swReverseEndPointTangentResult_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swReverseEndPointTangentResult_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swReverseEndPointTangentResult_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swReverseEndPointTangentResult_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swReverseEndPointTangent\_ConstraintConflict** | 2 = Reversing the end point tangent direction creates a conflict with existing constraints |
| **swReverseEndPointTangent\_InvalidSelection** | 1 = Select a valid end point tangent direction entity |
| **swReverseEndPointTangent\_Success** | 0 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)