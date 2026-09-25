<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis~GetSliverFacesCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| GetSliverFacesCount Method (IGeometryAnalysis) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IGeometryAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis.html) : GetSliverFacesCount Method (IGeometryAnalysis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*width*
:   Width to use to detect sliver faces

*errorcode*
:   Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

Gets the number of sliver faces in the part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSliverFacesCount( _    ByVal width As System.Double, _    ByRef errorcode As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGeometryAnalysis Dim width As System.Double Dim errorcode As System.Integer Dim value As System.Integer   value = instance.GetSliverFacesCount(width, errorcode) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSliverFacesCount(     System.double width,    out System.int errorcode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSliverFacesCount(  &   System.double width, &   [Out] System.int errorcode ) ``` | |

#### Parameters

*width*
:   Width to use to detect sliver faces

*errorcode*
:   Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

#### Return Value

Number of sliver faces

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IGeometryAnalysis::GetSliverFacesCount.

# ![](dotnetimages/collapse.gif)Example

[Analyze Geometry (VBA)](Analyze_Geometry_VB6.htm)

# ![](dotnetimages/collapse.gif)Remarks

Sliver faces are faces with a high aspect ratio (the ratio of length to width). A face is a sliver face if its area is less than the limiting area W\*((P/2)-W), where W is the specified width and P is the face perimeter.

# ![](dotnetimages/collapse.gif)See Also

####

[IGeometryAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis.html)

[IGeometryAnalysis Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2004 FCS