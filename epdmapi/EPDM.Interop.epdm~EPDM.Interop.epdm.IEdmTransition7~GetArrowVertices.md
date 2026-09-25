<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition7~GetArrowVertices.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetArrowVertices Method (IEdmTransition7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTransition7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition7.html) : GetArrowVertices Method (IEdmTransition7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoVertices*
:   Array of [EdmPoint](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmPoint.html) structures; one structure for each point that makes up the transition arrow

Gets the points that make up the transition arrow in the workflow graph.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetArrowVertices( _    ByRef ppoVertices() As EdmPoint _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetArrowVertices(     out EdmPoint[] ppoVertices ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetArrowVertices(  &   [Out] array<EdmPoint>^ ppoVertices ) ``` | |

#### Parameters

*ppoVertices*
:   Array of [EdmPoint](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmPoint.html) structures; one structure for each point that makes up the transition arrow

# ![](dotnetimages/collapse.gif)Example

See the [IEdmTransition7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition7.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTransition7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition7.html)

[IEdmTransition7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition7_members.html)

[IEdmTransition7::GetRect Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition7~GetRect.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011