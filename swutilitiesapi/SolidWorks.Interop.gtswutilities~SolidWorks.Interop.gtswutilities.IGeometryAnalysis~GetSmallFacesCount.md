<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis~GetSmallFacesCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| GetSmallFacesCount Method (IGeometryAnalysis) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IGeometryAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis.html) : GetSmallFacesCount Method (IGeometryAnalysis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*length*
:   Length to use to detect small faces

*errorcode*
:   Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

Gets the number of small faces on the part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSmallFacesCount( _    ByVal length As System.Double, _    ByRef errorcode As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGeometryAnalysis Dim length As System.Double Dim errorcode As System.Integer Dim value As System.Integer   value = instance.GetSmallFacesCount(length, errorcode) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSmallFacesCount(     System.double length,    out System.int errorcode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSmallFacesCount(  &   System.double length, &   [Out] System.int errorcode ) ``` | |

#### Parameters

*length*
:   Length to use to detect small faces

*errorcode*
:   Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

#### Return Value

Number of small faces

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IGeometryAnalysis::GetSmallFacesCount.

# ![](dotnetimages/collapse.gif)Example

[Analyze Geometry (VBA)](Analyze_Geometry_VB6.htm)

# ![](dotnetimages/collapse.gif)Remarks

Small faces are faces with all edges shorter than a specified length.

# ![](dotnetimages/collapse.gif)See Also

####

[IGeometryAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis.html)

[IGeometryAnalysis Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2004 FCS