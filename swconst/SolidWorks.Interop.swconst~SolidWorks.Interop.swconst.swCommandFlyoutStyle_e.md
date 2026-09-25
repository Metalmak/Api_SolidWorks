<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCommandFlyoutStyle_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCommandFlyoutStyle\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCommandFlyoutStyle\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Types of FlyoutGroup.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCommandFlyoutStyle_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCommandFlyoutStyle_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCommandFlyoutStyle_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCommandFlyoutStyle_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCommandFlyoutStyle\_Favorite** | 1 = the first command in the menu list is the immediate action for the main button |
| **swCommandFlyoutStyle\_LastUsed** | 2 = the last used command in the menu list is the immediate action for the main button |
| **swCommandFlyoutStyle\_Simple** | 0 = no immediate action is available for the main button |

# ![](dotnetimages/collapse.gif)Remarks

Context-sensitive menus support only the swCommandFlyoutStyle\_Simple flyout style.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)