<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAppCallBackCmd_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAppCallBackCmd\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAppCallBackCmd\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Types of application callback functions.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAppCallBackCmd_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAppCallBackCmd_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAppCallBackCmd_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAppCallBackCmd_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAppHelpContext** | 3 = Not used |
| **swAppIsCmdEnabled** | 4 = CommandGroup item is enabled |
| **swAppIsNewCmd** | 1 = True if data is new, false if not |
| **swAppPostNotifyEvent** | 5 = Your application is posting a callback to the SOLIDWORKS message queue that will be invoked when the callback is processed in the SOLIDWORKS message queue |
| **swAppWhatsNewDescription** | 2 = Interactive What's New |

# ![](dotnetimages/collapse.gif)Remarks

Use with ISldWorks::AddCallback.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)