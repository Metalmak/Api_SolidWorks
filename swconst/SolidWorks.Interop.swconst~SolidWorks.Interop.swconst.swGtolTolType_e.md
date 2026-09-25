<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swGtolTolType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swGtolTolType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swGtolTolType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Tolerance zone types in Gtol frame boxes.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swGtolTolType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swGtolTolType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swGtolTolType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swGtolTolType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swGtolTolType\_MAX** | 5 = Specifies a maximum value for a material condition that has already been specified as a modifier of the tolerance in the Gtol; this maximum upper tolerance is typically specified in the Tolerance 2 box with "MAX" |
| **swGtolTolType\_None** | 0 |
| **swGtolTolType\_ProjectedTolerance** | 2 = Applies to holes in which a pin, stud, or screw is to be inserted; controls the perpendicularity of the hole to the extent of the projection from the hole; specified with a circle-P symbol; typically a height is also specified in a separate field |
| **swGtolTolType\_Square** | 3 |
| **swGtolTolType\_UnequallyDisposedProfile** | 4 = Indicates that the profile of a surface tolerance is not symmetrical about the true profile; the value following the circle-U symbol is the amount of the tolerance that is in a direction that would allow additional material to be added to the true profile |
| **swGtolTolType\_Unknown** | 1 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)