<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCornerReliefSuitCaseType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCornerReliefSuitCaseType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCornerReliefSuitCaseType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sheet metal corner relief suitcase types.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCornerReliefSuitCaseType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCornerReliefSuitCaseType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCornerReliefSuitCaseType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCornerReliefSuitCaseType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCornerReliefSuitCase\_Default** | 0 = Leaves the gap unchanged |
| **swCornerReliefSuitCase\_ExtendGapInBendArea** | 1 = Cut the corner relief with the gap |
| **swCornerReliefSuitCase\_FillInSomeGap** | 2 = Extends the corner relief material into the gap |

# ![](dotnetimages/collapse.gif)Remarks

A suitcase is a closed spherical corner without any cutouts.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)