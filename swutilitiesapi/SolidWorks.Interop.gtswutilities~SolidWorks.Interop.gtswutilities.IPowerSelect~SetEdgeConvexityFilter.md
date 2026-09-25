<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~SetEdgeConvexityFilter.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| SetEdgeConvexityFilter Method (IPowerSelect) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html) : SetEdgeConvexityFilter Method (IPowerSelect) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*bConvex*
:   True to get convex edges, false to not

*bConcave*
:   True to get concave edges, false to not

*bIgnoreMixedLoop*
:   True to ignore loops with convex or concave edges, false to not

Sets the Edge convexity filter for this PowerSelect session.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetEdgeConvexityFilter( _    ByVal bConvex As System.Boolean, _    ByVal bConcave As System.Boolean, _    ByVal bIgnoreMixedLoop As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPowerSelect Dim bConvex As System.Boolean Dim bConcave As System.Boolean Dim bIgnoreMixedLoop As System.Boolean Dim value As System.Integer   value = instance.SetEdgeConvexityFilter(bConvex, bConcave, bIgnoreMixedLoop) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetEdgeConvexityFilter(     System.bool bConvex,    System.bool bConcave,    System.bool bIgnoreMixedLoop ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetEdgeConvexityFilter(  &   System.bool bConvex, &   System.bool bConcave, &   System.bool bIgnoreMixedLoop ) ``` | |

#### Parameters

*bConvex*
:   True to get convex edges, false to not

*bConcave*
:   True to get concave edges, false to not

*bIgnoreMixedLoop*
:   True to ignore loops with convex or concave edges, false to not

#### Return Value

Error as defined in [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IPowerSelect::SetEdgeConvexityFilter.

# ![](dotnetimages/collapse.gif)Example

[Run PowerSelect (VBA)](Run_PowerSelect_VB6.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html)

[IPowerSelect Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect_members.html)

[IPowerSelect::GetEdgeConvexityFilter Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~GetEdgeConvexityFilter.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2005 FCS