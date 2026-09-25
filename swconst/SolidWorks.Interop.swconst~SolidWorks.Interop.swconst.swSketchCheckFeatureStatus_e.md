<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSketchCheckFeatureStatus_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSketchCheckFeatureStatus\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSketchCheckFeatureStatus\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Statuses after checking to see if this sketch is valid for use in creating the specified feature

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSketchCheckFeatureStatus_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSketchCheckFeatureStatus_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSketchCheckFeatureStatus_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSketchCheckFeatureStatus_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSketchCheckFeatureStatus\_ClosedWantOpen** | 15 = The contour is closed |
| **swSketchCheckFeatureStatus\_ContourIntersectsCenterLine** | 23 = The revolution contour cannot cross the centerline or touch it in an isolated point |
| **swSketchCheckFeatureStatus\_CturXCtur** | 12 = The sketch has intersecting contours |
| **swSketchCheckFeatureStatus\_DisjCturs** | 13 = The sketch contains disjoint contours |
| **swSketchCheckFeatureStatus\_DoubleContainment** | 16 = The sketch contains a doubly nested contour |
| **swSketchCheckFeatureStatus\_EmptySketch** | 5 |
| **swSketchCheckFeatureStatus\_EntUnspecBad** | 3 = The sketch contains a self-intersecting entity |
| **swSketchCheckFeatureStatus\_EntXEnt** | 1 = The sketch contains a self-intersecting contour |
| **swSketchCheckFeatureStatus\_EntXSelf** | 2 = The sketch contains a self-intersecting entity |
| **swSketchCheckFeatureStatus\_ManyOpen** | 9 = The sketch has more than one open contour |
| **swSketchCheckFeatureStatus\_MixedContours** | 11 = The sketch has both open and closed contours |
| **swSketchCheckFeatureStatus\_MoreThanOneContour** | 17 = The sketch contains more than one contour |
| **swSketchCheckFeatureStatus\_NeedsAxis** | 21 = The sketch should contain a centerline |
| **swSketchCheckFeatureStatus\_NoOpen** | 10 = The sketch has no more open contours |
| **swSketchCheckFeatureStatus\_OK** | 0 = No problems found, the sketch can be used to create the specified feature. |
| **swSketchCheckFeatureStatus\_OneClosedContourExpected** | 19 = The sketch should contain a single closed contour |
| **swSketchCheckFeatureStatus\_OneOpenContourExpected** | 18 = The sketch should contain a single open contour |
| **swSketchCheckFeatureStatus\_OpenOrUnclear** | 22 = Selected contours are open or ambiguous |
| **swSketchCheckFeatureStatus\_OpenWantClosed** | 14 = The contour is open |
| **swSketchCheckFeatureStatus\_ThreeEnts** | 4 = The sketch cannot be used for a feature because an endpoint is wrongly shared by multiple entities |
| **swSketchCheckFeatureStatus\_UnknownError** | -1 = Unknown error |
| **swSketchCheckFeatureStatus\_WantSingleOpenOrMultiClosedDisjoint** | 20 = The sketch should contain either one open contour or multiple closed disjoint contours |
| **swSketchCheckFeatureStatus\_WrongManyContours** | 7 = The sketch has more than one contour |
| **swSketchCheckFeatureStatus\_WrongOpen** | 6 = The sketch contains an open contour |
| **swSketchCheckFeatureStatus\_ZeroLengthEnt** | 8 = The sketch contains a zero-length entity |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)