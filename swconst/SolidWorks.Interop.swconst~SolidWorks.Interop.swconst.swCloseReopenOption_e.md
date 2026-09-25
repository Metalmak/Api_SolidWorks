<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCloseReopenOption_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCloseReopenOption\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCloseReopenOption\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

File close and reopen options. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCloseReopenOption_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCloseReopenOption_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCloseReopenOption_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCloseReopenOption_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCloseReopenOption\_DiscardChanges** | 2 or 0x2; include this option to discard any changes to the document before reopening it; if you exclude this option and there are changes, ISldWorks::CloseAndReopen fails and returns [swCloseReopenError\_e.swCloseReopenModifiedError](SOLIDWORKS.Interop.swconst~SOLIDWORKS.Interop.swconst.swCloseReopenError_e.html) |
| **swCloseReopenOption\_ExitDetailingMode** | 8 or 0x8; include this option to reopen model drawings as resolved; if excluded by ISldWorks::CloseAndReopen2, keeps a model drawing in detailing mode on reopen |
| **swCloseReopenOption\_MatchSheet** | 4 or 0x4; include this option to open the same sheet that was active during closing |
| **swCloseReopenOption\_ReadOnly** | 1 or 0x1; include this option to open the drawing document in read-only mode |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)