<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFlangeOffsetTypes_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFlangeOffsetTypes\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFlangeOffsetTypes\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

End conditions for both flange length and flange position offset for sheet metal edge and base flanges.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFlangeOffsetTypes_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFlangeOffsetTypes_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFlangeOffsetTypes_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFlangeOffsetTypes_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swFlangeOffsetBlind** | 1 = Positions the edge flange based on the length and direction you specify |
| **swFlangeOffsetFromSurface** | 4 |
| **swFlangeOffsetMidPlane** | 5 |
| **swFlangeOffsetUptoEdgeAndMerge** | 6 = Creates the edge flange in a multibody part by merging a selected edge on one body with an Up To reference edge on the second body |
| **swFlangeOffsetUpToSurface** | 3 |
| **swFlangeOffsetUpToVertex** | 2 = Positions the edge flange up to a specified vertex; for flange length, the selected vertex may be either on a plane that is normal to the end face of the edge flange or on a plane that is parallel to the face of the base flange |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)