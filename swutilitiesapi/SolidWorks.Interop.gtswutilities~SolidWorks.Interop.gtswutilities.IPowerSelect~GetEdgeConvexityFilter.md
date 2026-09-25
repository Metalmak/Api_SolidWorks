<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~GetEdgeConvexityFilter.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| GetEdgeConvexityFilter Method (IPowerSelect) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html) : GetEdgeConvexityFilter Method (IPowerSelect) |

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

Gets the Edge convexity filter set in this PowerSelect session.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEdgeConvexityFilter( _    ByRef bConvex As System.Boolean, _    ByRef bConcave As System.Boolean, _    ByRef bIgnoreMixedLoop As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPowerSelect Dim bConvex As System.Boolean Dim bConcave As System.Boolean Dim bIgnoreMixedLoop As System.Boolean Dim value As System.Integer   value = instance.GetEdgeConvexityFilter(bConvex, bConcave, bIgnoreMixedLoop) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetEdgeConvexityFilter(     out System.bool bConvex,    out System.bool bConcave,    out System.bool bIgnoreMixedLoop ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetEdgeConvexityFilter(  &   [Out] System.bool bConvex, &   [Out] System.bool bConcave, &   [Out] System.bool bIgnoreMixedLoop ) ``` | |

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

See IPowerSelect::GetEdgeConvexityFilter.

# ![](dotnetimages/collapse.gif)See Also

####

[IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html)

[IPowerSelect Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect_members.html)

[IPowerSelect::SetEdgeConvexityFilter Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~SetEdgeConvexityFilter.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2005 FCS