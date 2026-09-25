<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IMakeIsoCurves.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMakeIsoCurves Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : IMakeIsoCurves Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UvRange*
:   Array of 4 doubles indicating the range of the surface to use (see **Remarks**)

*Dir*
:   Array of 3 doubles indicating the direction of projection on the surface (see Remarks)

*Angle*
:   Angle relative to dir where to create the curves

*Tol*
:   Tolerance of the curves

*CurveCount*
:   Number of curves to create (see Remarks)

*Curves*
:   Array of [curves](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) of size CurveCount

*CurveBounds*
:   Array of doubles of size 2\*Curves indicating the parametric bounds of the curve

Creates curves on a surface.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IMakeIsoCurves( _    ByRef UvRange As System.Double, _    ByRef Dir As System.Double, _    ByVal Angle As System.Double, _    ByVal Tol As System.Double, _    ByVal CurveCount As System.Integer, _    ByRef Curves As Curve, _    ByRef CurveBounds As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim UvRange As System.Double Dim Dir As System.Double Dim Angle As System.Double Dim Tol As System.Double Dim CurveCount As System.Integer Dim Curves As Curve Dim CurveBounds As System.Double Dim value As System.Boolean   value = instance.IMakeIsoCurves(UvRange, Dir, Angle, Tol, CurveCount, Curves, CurveBounds) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IMakeIsoCurves(     ref System.double UvRange,    ref System.double Dir,    System.double Angle,    System.double Tol,    System.int CurveCount,    out Curve Curves,    out System.double CurveBounds ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IMakeIsoCurves(  &   System.double% UvRange, &   System.double% Dir, &   System.double Angle, &   System.double Tol, &   System.int CurveCount, &   [Out] Curve^ Curves, &   [Out] System.double CurveBounds ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UvRange*
:   Array of 4 doubles indicating the range of the surface to use (see **Remarks**)

*Dir*
:   Array of 3 doubles indicating the direction of projection on the surface (see Remarks)

*Angle*
:   Angle relative to dir where to create the curves

*Tol*
:   Tolerance of the curves

*CurveCount*
:   Number of curves to create (see Remarks)

*Curves*
:   Array of [curves](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) of size CurveCount

*CurveBounds*
:   Array of doubles of size 2\*Curves indicating the parametric bounds of the curve

#### Return Value

True if curves are created on the surface, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::IMakeIsoCurves.

# ![](dotnetimages/collapse.gif)Remarks

The UvRange argument is an array of 4 doubles indicating the minimum and maximum U and V values:

[ u\_min, u\_max, v\_min, v\_max ]

The dir argument is an array of 3 doubles representing the unit vector:

[ x, y, z ]

Before calling this method, call [ISurface::IGetMakeIsoCurvesCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IGetMakeIsoCurvesCount.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

[ISurface::MakeIsoCurves Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~MakeIsoCurves.html)

[ISurface::MakeIsoCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~MakeIsoCurve.html)

[ISurface::IMakeIsoCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IMakeIsoCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP2, Revision Number 12.2