<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swMatesDefaultMisalignment_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swMatesDefaultMisalignment\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swMatesDefaultMisalignment\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Concentric mate misalignment options.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swMatesDefaultMisalignment_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swMatesDefaultMisalignment_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swMatesDefaultMisalignment_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swMatesDefaultMisalignment_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swMatesAlignFirstConcentricMate** | 0; Align this mate; align the mate currently being edited to be exactly concentric, causing the linked mate to be misaligned |
| **swMatesAlignSecondConcentricMate** | 1; Align linked mate; aligns the linked mate to be exactly concentric, causing the currently edited mate to be misaligned |
| **swMatesSymmetric** | 2; Symmetric; misaligns both concentric mates, splitting the deviation evenly between mates |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)