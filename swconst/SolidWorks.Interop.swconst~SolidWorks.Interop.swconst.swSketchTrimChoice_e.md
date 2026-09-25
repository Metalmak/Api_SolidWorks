<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSketchTrimChoice_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSketchTrimChoice\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSketchTrimChoice\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sketch trim options.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSketchTrimChoice_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSketchTrimChoice_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSketchTrimChoice_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSketchTrimChoice_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSketchTrimClosest** | 0 = Trim to closest. One and only one sketch segment must be selected before calling ISketchManager::SketchTrim using this option. |
| **swSketchTrimCorner** | 1 = Corner. Two and only two sketch segments must be selected before calling ISketchManager::SketchTrim using this option. |
| **swSketchTrimEntities** | 4 = Power trim. Before calling ISketchManager::SketchTrim using this option, use IModelDocExtension::SelectByID2 with Mark = 2 to select 1 or more sketch segments (up to total number of sketch segments in the model), specifying their pick points. The sketch segments are trimmed to the sketch segments nearest their pick points.  When you trim sketch segments using Power trim in the user interface, you drag your cursor across sketch segments, and the point at which the cursor crosses a sketch segment is where that sketch segment is trimmed. The API simulates this functionality by requiring you to select sketch segments by pick points, which are used as references when trimming the selected sketch segments. |
| **swSketchTrimEntityPoint** | 3 = Power trim. One and only one sketch segment must be selected before calling ISketchManager::SketchTrim using this option. Trims to a specific point on the sketch segment. Call this method, specifying non-zero X, Y, and Z, the point at which to trim the selected sketch segment. The specified point must lie on the sketch segment. |
| **swSketchTrimInside** | 6 = Trim away inside. Before calling ISketchManager::SketchTrim using this option, select at least three sketch segments: two to create the boundary, and one or more that intersect both sketch segments in the boundary. All selected sketch segments that intersect the boundary are trimmed inside the boundary segments. |
| **swSketchTrimOutside** | 5 = Trim away outside. Before calling ISketchManager::SketchTrim using this option, select at least three sketch segments: two to create the trim boundary, and one or more that intersect both sketch segments in the boundary. All selected sketch segments that intersect the boundary are trimmed outside the boundary segments. |
| **swSketchTrimTwoEntities** | 2 = Power trim. Before calling ISketchManager::SketchTrim using this option, use IModelDocExtension::SelectByID2 with Mark = 0 to select two intersecting sketch segments, specifying their pick points. Trims the first selected sketch segment to the second intersecting sketch segment. The order in which the sketch segments are selected determines which one is trimmed. The first selected sketch segment will be trimmed on its pick point side to the second selected sketch segment. |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)