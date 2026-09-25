<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swRayPtsResults_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swRayPtsResults\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swRayPtsResults\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Types of intersections and whether the rays are entering or exiting the body when they hit. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swRayPtsResults_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swRayPtsResults_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swRayPtsResults_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swRayPtsResults_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swRayPtsResultsEDGE** | 4 or 0x4; Edge hit |
| **swRayPtsResultsENTER** | 16 or 0x10; Ray was entering body when it hit (optionally appears when swRayPtsOptsENTRY\_EXIT is specified in the options argument to IModelDoc2::RayIntersections) |
| **swRayPtsResultsEXIT** | 32 or 0x20; Ray was exiting body when it hit (optionally appears when swRayPtsOptsENTRY\_EXIT is specified in the options argument to IModelDoc2::RayIntersections) |
| **swRayPtsResultsFACE** | 1 or 0x1; Simple face hit |
| **swRayPtsResultsSILHOUETTE** | 2 or 0x2; Grazing face hit |
| **swRayPtsResultsUnknown** | 0 or 0x0; Unknown |
| **swRayPtsResultsVERTEX** | 8 or 0x8; Vertex hit |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)