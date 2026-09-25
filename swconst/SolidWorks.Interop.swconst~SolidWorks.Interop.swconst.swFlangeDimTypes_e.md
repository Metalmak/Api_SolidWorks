<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFlangeDimTypes_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFlangeDimTypes\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFlangeDimTypes\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Origins for dimensioning Blind or Up To Edge And Merge flange length end conditions in edge flanges.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFlangeDimTypes_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFlangeDimTypes_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFlangeDimTypes_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFlangeDimTypes_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swFlangeDimTypeBendTangentArc** | 3 = Flange length is measured from the edge flange face to a line that is tangent to the bend; not valid for the Up To Edge And Merge length end condition |
| **swFlangeDimTypeInnerVirtualSharp** | 2 = Flange length is measured from the edge flange face to an inner virtual sharp (sketch point at the virtual intersection point of two sketch entities) |
| **swFlangeDimTypeOuterVirtualSharp** | 1 = Flange length is measured from the edge flange face to an outer virtual sharp (sketch point at the virtual intersection point of two sketch entities) |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)