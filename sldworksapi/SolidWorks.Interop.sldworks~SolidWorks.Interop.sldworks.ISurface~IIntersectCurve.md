<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IIntersectCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IIntersectCurve Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : IIntersectCurve Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OtherCurve*

*CurveBound*

*PointCount*

*PointArray*

*TArray*

*UvArray*

Obsolete. Superseded by [ISurface::IIntersectCurve2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IIntersectCurve2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IIntersectCurve( _    ByVal OtherCurve As Curve, _    ByRef CurveBound As System.Double, _    ByVal PointCount As System.Integer, _    ByRef PointArray As System.Double, _    ByRef TArray As System.Double, _    ByRef UvArray As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim OtherCurve As Curve Dim CurveBound As System.Double Dim PointCount As System.Integer Dim PointArray As System.Double Dim TArray As System.Double Dim UvArray As System.Double Dim value As System.Boolean   value = instance.IIntersectCurve(OtherCurve, CurveBound, PointCount, PointArray, TArray, UvArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IIntersectCurve(     Curve OtherCurve,    ref System.double CurveBound,    System.int PointCount,    out System.double PointArray,    out System.double TArray,    out System.double UvArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IIntersectCurve(  &   Curve^ OtherCurve, &   System.double% CurveBound, &   System.int PointCount, &   [Out] System.double PointArray, &   [Out] System.double TArray, &   [Out] System.double UvArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OtherCurve*

*CurveBound*

*PointCount*

*PointArray*

*TArray*

*UvArray*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::IIntersectCurve.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)