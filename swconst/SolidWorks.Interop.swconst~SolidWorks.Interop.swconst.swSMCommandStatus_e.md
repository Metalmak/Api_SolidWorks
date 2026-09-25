<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSMCommandStatus_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSMCommandStatus\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSMCommandStatus\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Return conditions for various sheet metal APIs that attempt to do set operations.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSMCommandStatus_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSMCommandStatus_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSMCommandStatus_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSMCommandStatus_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSMErrorInvalidBendState** | 4 = Failed, an invalid bend state was specified |
| **swSMErrorNone** | 0 = Successful, operation completed |
| **swSMErrorNotAPart** | 2 = Failed, sheet metal commands only apply to SOLIDWORKS parts |
| **swSMErrorNotASheetMetalPart** | 3 = Failed, the part contains no sheet metal features |
| **swSMErrorUnknown** | 1 = Failed, for an unknown reason |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)