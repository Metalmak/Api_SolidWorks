<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAutodimScheme_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAutodimScheme\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAutodimScheme\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Dimensioning schemes for ISketch::AutoDimension2 and IDrawingDoc::AutoDimension.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAutodimScheme_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAutodimScheme_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAutodimScheme_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAutodimScheme_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAutodimSchemeBaseline** | 1 = Use a baseline dimensioning scheme |
| **swAutodimSchemeCenterline** | 4 = Not supported in sketches or drawings; do not use |
| **swAutodimSchemeChain** | 3 = Use a chain dimensioning scheme |
| **swAutodimSchemeOrdinate** | 2 = Use an ordinate dimensioning scheme |

# ![](dotnetimages/collapse.gif)Remarks

The horizontal and vertical dimension placements are specified independently using the HorizontalPlacement and VerticalPlacement parameters in the methods.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)