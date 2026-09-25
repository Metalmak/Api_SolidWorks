<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSaveItemsPathError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSaveItemsPathError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSaveItemsPathError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Error return codes for IAdvancedSaveAsOptions::ModifyItemsNameAndPath.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSaveItemsPathError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSaveItemsPathError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSaveItemsPathError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSaveItemsPathError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSaveItemsPathError\_ArraySizeNotMatching** | 1 = Input arrays must be the same size |
| **swSaveItemsPathError\_InvalidPath** | 2 = Path provided does not exist or user does not have write access |
| **swSaveItemsPathError\_Succeeded** | 0 |
| **swSaveItemsPathError\_WrongComponentName** | 3 = Name provided is not supported by SOLIDWORKS |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)