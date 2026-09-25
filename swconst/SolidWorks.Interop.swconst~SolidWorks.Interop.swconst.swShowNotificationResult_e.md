<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swShowNotificationResult_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swShowNotificationResult\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swShowNotificationResult\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

User notification display return values.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swShowNotificationResult_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swShowNotificationResult_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swShowNotificationResult_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swShowNotificationResult_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swShowNotificationResult\_DontShowAgain** | 1 = The user notification is not shown when "Don't show again" is selected |
| **swShowNotificationResult\_FailedInvalidDefinition** | 2 = The user notification could not be displayed due to an invalid definition (e.g., empty title/description) |
| **swShowNotificationResult\_FailedInvalidHandler** | 3 = The user notification could not be desiplayed because the Handler argument is NULL or does not support the expected interface |
| **swShowNotificationResult\_Shown** | 0 = The user notification is shown |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)