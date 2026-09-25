<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swEdgeFlangeError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swEdgeFlangeError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swEdgeFlangeError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Edge flange error codes.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swEdgeFlangeError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swEdgeFlangeError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swEdgeFlangeError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swEdgeFlangeError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swEdgeFlangeError\_EdgeAlreadyExists** | 4 = Specified edge already exists |
| **swEdgeFlangeError\_EdgeNotSpecified** | 1 = Input array of edges is empty |
| **swEdgeFlangeError\_GenericError** | 7 = Unknown error |
| **swEdgeFlangeError\_InvalidEdge** | 5 = Specified edge is invalid |
| **swEdgeFlangeError\_MustSpecifyAtLeastOneEdge** | 6 = You must specify at least one edge |
| **swEdgeFlangeError\_NoError** | 0 = No error |
| **swEdgeFlangeError\_NumberOfEdgesAndSketchesNotEqual** | 3 = Number of edges must equal the number of sketches |
| **swEdgeFlangeError\_SketchNotSpecified** | 2 = Input array of sketches is empty |

# ![](dotnetimages/collapse.gif)Remarks

These error codes are returned by IEdgeFlangeFeatureData::AddEdges and IEdgeFlangeFeatureData::RemoveEdges.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)