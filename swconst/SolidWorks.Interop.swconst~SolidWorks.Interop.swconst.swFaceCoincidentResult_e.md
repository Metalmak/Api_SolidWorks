<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFaceCoincidentResult_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFaceCoincidentResult\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFaceCoincidentResult\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Face coincidence results.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFaceCoincidentResult_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFaceCoincidentResult_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFaceCoincidentResult_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFaceCoincidentResult_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swFaceCoincident\_FalseBoundary1** | 3 = The two faces are not coincident. At least one point on the boundary of face 1 is not coincident with the boundary of face 2. |
| **swFaceCoincident\_FalseBoundary2** | 4 = The two faces are not coincident. At least one point on the boundary of face 2 is not coincident with the boundary of face 1. |
| **swFaceCoincident\_FalseFace1** | 5 = The two faces are not coincident. At least one point on face 1 is not coincident with face 2. |
| **swFaceCoincident\_FalseFace2** | 6 = The two faces are not coincident. At least one point on face 2 is not coincident with face 1. |
| **swFaceCoincident\_FalseSurface** | 7 = At least one of the faces does not have a surface attached. |
| **swFaceCoincident\_FalseTopology** | 2 = The two faces are not coincident. The number of holes are different. |
| **swFaceCoincident\_True** | 0 = The faces are coincident to the specified tolerance. |
| **swFaceCoincident\_TrueReversed** | 1 = The two faces are coincident to the specified tolerance, but their normals are reversed. |
| **swFaceCoincidentUnknownResult** | -1 = Unknown |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)