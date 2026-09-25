<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swEdrawingsAttachmentOption_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swEdrawingsAttachmentOption\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swEdrawingsAttachmentOption\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Configuration options for creating and attaching STEP files when publishing a part or assembly to eDrawings.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swEdrawingsAttachmentOption_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swEdrawingsAttachmentOption_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swEdrawingsAttachmentOption_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swEdrawingsAttachmentOption_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swEdrawingsAttachActive** | 1 = Create and attach STEP files to the active configuration only |
| **swEdrawingsAttachAll** | 2 = Create and attach STEP files to all configurations |
| **swEdrawingsAttachNone** | 0 = Do not create and attach any STEP files |
| **swEdrawingsAttachSelected** | 3 = Create and attach STEP files to specified configurations only |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)