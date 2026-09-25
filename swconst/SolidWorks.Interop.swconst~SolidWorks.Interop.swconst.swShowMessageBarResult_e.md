<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swShowMessageBarResult_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swShowMessageBarResult\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swShowMessageBarResult\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Message bar display result codes.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swShowMessageBarResult_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swShowMessageBarResult_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swShowMessageBarResult_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swShowMessageBarResult_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swShowMessageBarResult\_DontShowAgain** | 1 = The message bar is not shown when "Don't show again" is selected |
| **swShowMessageBarResult\_FailedInvalidDefinition** | 2 = The message bar could not be displayed due to an invalid definition (e.g., empty title/description) |
| **swShowMessageBarResult\_FailedInvalidHandler** | 3 = The message bar could not be desiplayed because the Handler argument is NULL or does not support the expected interface |
| **swShowMessageBarResult\_Shown** | 0 = The modeless message bar is shown |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)