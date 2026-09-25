<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IntersectCurve2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IntersectCurve2 Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : IntersectCurve2 Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OtherCurve*
:   [Curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

*CurveBound*
:   Array of 6 doubles representing the start and end points of the curve

*PointArray*
:   Array of points

*TArray*
:   Array of parameters on curve

*UvArray*
:   Array of parameters on surface

Gets a surface-curve intersection.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IntersectCurve2( _    ByVal OtherCurve As System.Object, _    ByVal CurveBound As System.Object, _    ByRef PointArray As System.Object, _    ByRef TArray As System.Object, _    ByRef UvArray As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim OtherCurve As System.Object Dim CurveBound As System.Object Dim PointArray As System.Object Dim TArray As System.Object Dim UvArray As System.Object Dim value As System.Boolean   value = instance.IntersectCurve2(OtherCurve, CurveBound, PointArray, TArray, UvArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IntersectCurve2(     System.object OtherCurve,    System.object CurveBound,    out System.object PointArray,    out System.object TArray,    out System.object UvArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IntersectCurve2(  &   System.Object^ OtherCurve, &   System.Object^ CurveBound, &   [Out] System.Object^ PointArray, &   [Out] System.Object^ TArray, &   [Out] System.Object^ UvArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OtherCurve*
:   [Curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

*CurveBound*
:   Array of 6 doubles representing the start and end points of the curve

*PointArray*
:   Array of points

*TArray*
:   Array of parameters on curve

*UvArray*
:   Array of parameters on surface

#### Return Value

True if getting the intersection succeeded, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::IntersectCurve2.

# ![](dotnetimages/collapse.gif)Remarks

The curves must be bounded.

Visual Basic and C++ Dispatch applications should use this method instead of using [ISurface::GetIntersectCurveCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~GetIntersectCurveCount2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

[ISurface::IIntersectCurve2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IIntersectCurve2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0