<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis~GetKnifeEdgesCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| GetKnifeEdgesCount Method (IGeometryAnalysis) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IGeometryAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis.html) : GetKnifeEdgesCount Method (IGeometryAnalysis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*angle*
:   Angle to use to determine the knife edges

*errorcode*
:   Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

Gets the number of knife edges in the part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetKnifeEdgesCount( _    ByVal angle As System.Double, _    ByRef errorcode As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGeometryAnalysis Dim angle As System.Double Dim errorcode As System.Integer Dim value As System.Integer   value = instance.GetKnifeEdgesCount(angle, errorcode) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetKnifeEdgesCount(     System.double angle,    out System.int errorcode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetKnifeEdgesCount(  &   System.double angle, &   [Out] System.int errorcode ) ``` | |

#### Parameters

*angle*
:   Angle to use to determine the knife edges

*errorcode*
:   Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

#### Return Value

Number of knife edges

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IGeometryAnalysis::GetKnifeEdgesCount.

# ![](dotnetimages/collapse.gif)Example

[Analyze Geometry (VBA)](Analyze_Geometry_VB6.htm)

# ![](dotnetimages/collapse.gif)Remarks

A sharp edge or knife edge is an edge where the angle between two adjacent faces
is acute.

# ![](dotnetimages/collapse.gif)See Also

####

[IGeometryAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis.html)

[IGeometryAnalysis Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2004 FCS