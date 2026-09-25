<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swHandleWindowFromHandleCreationFailure_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swHandleWindowFromHandleCreationFailure\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swHandleWindowFromHandleCreationFailure\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Actions on failure to create a .NET control on a PropertyManager page.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swHandleWindowFromHandleCreationFailure_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swHandleWindowFromHandleCreationFailure_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swHandleWindowFromHandleCreationFailure_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swHandleWindowFromHandleCreationFailure_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swHandleWindowFromHandleCreationFailure\_Cancel** | 1 = Create the PropertyManager page without the .NET control. (default) |
| **swHandleWindowFromHandleCreationFailure\_Continue** | 3 = Cancel the creation of the PropertyManager page. |
| **swHandleWindowFromHandleCreationFailure\_Retry** | 2 = Try to create the .NET control again. |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)