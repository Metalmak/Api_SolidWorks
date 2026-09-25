<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swArrowPlacement_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swArrowPlacement\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swArrowPlacement\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Smart arrow placement.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swArrowPlacement_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swArrowPlacement_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swArrowPlacement_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swArrowPlacement_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swArrowPlacementLegacy** | 0 = Vary Smart arrow placement as in SOLIDWORKS 2012 and earlier (see **Remarks**) |
| **swArrowPlacementSmartArrowFollowText** | 1 |
| **swArrowPlacementSmartArrowRemainAttachedToArc** | 2 |

# ![](dotnetimages/collapse.gif)Remarks

In SOLIDWORKS 2012 and earlier, Smart arrows sometimes:

* Remained on the far side of an arc when moved to its other side.* Were attached to an extension line.* Pointed out to space.* Were placed on the part.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)