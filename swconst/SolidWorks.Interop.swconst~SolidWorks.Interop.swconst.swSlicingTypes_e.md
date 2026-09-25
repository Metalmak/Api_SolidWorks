<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSlicingTypes_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSlicingTypes\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSlicingTypes\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Types of slicing. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSlicingTypes_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSlicingTypes_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSlicingTypes_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSlicingTypes_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSlicingTypes\_Circle** | 4 = Creates a circle whose diameter equals the average of the length and width of the rectangle that encloses all the sketch entities; circle is located at the intersection of the source geometry and the slicing plane |
| **swSlicingTypes\_Exact** | 2 = Creates an exact intersection of the mesh BREP body and graphics body resulting in a polyline; set only if swSlicingTypes\_Intersection is also set; not valid with swSlicingTypes\_Circle and swSlicingTypes\_Rectangle |
| **swSlicingTypes\_Intersection** | 1 = For SOLIDWORKS BREP geometry, the slicing is identical to what is generated using the Intersection Curve tool; for mesh BREP and graphics bodies, sketches generated cannot be modified |
| **swSlicingTypes\_None** | 0 |
| **swSlicingTypes\_Rectangle** | 8 = Creates a rectangle that encloses all the sketch entities and is located at the intersection of the source geometry and the slicing plane |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)