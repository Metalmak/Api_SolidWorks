<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swConstrainedCornerAction_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swConstrainedCornerAction\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swConstrainedCornerAction\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Actions to take if the corner to be filleted is constrained or has a dimension.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swConstrainedCornerAction_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swConstrainedCornerAction_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swConstrainedCornerAction_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swConstrainedCornerAction_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swConstrainedCornerDeleteGeometry** | 2 = Delete the constraint or dimension and add the fillet |
| **swConstrainedCornerInteract** | 0 = Ask the user whether to delete the geometry or stop processing |
| **swConstrainedCornerKeepGeometry** | 1 = Keep the constraint or dimension by creating a virtual intersection point before adding the fillet |
| **swConstrainedCornerStopProcessing** | 3 = Do not delete the constraint or dimension and do not create the fillet |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)