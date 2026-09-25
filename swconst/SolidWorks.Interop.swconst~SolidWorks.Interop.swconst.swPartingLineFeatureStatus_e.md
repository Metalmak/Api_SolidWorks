<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swPartingLineFeatureStatus_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swPartingLineFeatureStatus\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swPartingLineFeatureStatus\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Statuses of parting line features.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swPartingLineFeatureStatus_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swPartingLineFeatureStatus_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swPartingLineFeatureStatus_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swPartingLineFeatureStatus_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **STATUS\_MOLD\_PARTINGLINE\_EDGES\_OPEN** | 2 = Select edges that form a closed loop |
| **STATUS\_MOLD\_PARTINGLINE\_NON\_SEPARABLE** | 4 = The parting line is complete, but the mold cannot be separated into core and cavity; you might need to create shut-off surfaces |
| **STATUS\_MOLD\_PARTINGLINE\_SEPARABLE** | 3 = The parting line is complete; the mold can be separated into core and cavity |
| **STATUS\_MOLD\_REDUNDANT\_EDGES** | 1 = There are more than enough edges selected to form a parting line; remove any redundant edges or add edges to close gaps between disjoint edge chains |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)