<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAddToRecentDocumentList_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAddToRecentDocumentList\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAddToRecentDocumentList\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Recent Document list actions when opening a document using ISldWorks::OpenDoc7 with IDocumentSpecification::AddToRecentDocumentList.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAddToRecentDocumentList_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAddToRecentDocumentList_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAddToRecentDocumentList_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAddToRecentDocumentList_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAddToRecentDocumentList\_Add** | 1 |
| **swAddToRecentDocumentList\_Default** | 0 = Default OpenDoc7 action: if a configuration is specified, the document is not added to the Recent Documents list; if a configuration is not specified, the document is added |
| **swAddToRecentDocumentList\_DontAdd** | 2 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)