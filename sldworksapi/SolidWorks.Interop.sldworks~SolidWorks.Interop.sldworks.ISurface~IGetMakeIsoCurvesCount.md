<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IGetMakeIsoCurvesCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetMakeIsoCurvesCount Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : IGetMakeIsoCurvesCount Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UvRange*
:   Array of 4 doubles indicating the range of surface to use (see **Remarks**)

*Dir*
:   Array of 3 doubles indicating the direction of the projection on the surface (see
    Remarks)

*Angle*
:   Angle relative to Dir where to create the curves

*Tol*
:   Tolerance of the curves to create

Gets the number of curves that represent the ISO line of a given direction.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetMakeIsoCurvesCount( _    ByRef UvRange As System.Double, _    ByRef Dir As System.Double, _    ByVal Angle As System.Double, _    ByVal Tol As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim UvRange As System.Double Dim Dir As System.Double Dim Angle As System.Double Dim Tol As System.Double Dim value As System.Integer   value = instance.IGetMakeIsoCurvesCount(UvRange, Dir, Angle, Tol) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetMakeIsoCurvesCount(     ref System.double UvRange,    ref System.double Dir,    System.double Angle,    System.double Tol ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetMakeIsoCurvesCount(  &   System.double% UvRange, &   System.double% Dir, &   System.double Angle, &   System.double Tol ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UvRange*
:   Array of 4 doubles indicating the range of surface to use (see **Remarks**)

*Dir*
:   Array of 3 doubles indicating the direction of the projection on the surface (see
    Remarks)

*Angle*
:   Angle relative to Dir where to create the curves

*Tol*
:   Tolerance of the curves to create

#### Return Value

Number of curves to create

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::IGetMakeIsoCurvesCount.

# ![](dotnetimages/collapse.gif)Remarks

The uvRange argument is an array of 4 doubles indicating the minimum and maximum U and V values:

> [ u\_min, u\_max, v\_min, v\_max ]

The dir argument is an array of 3 doubles representing the unit vector:

> [ x, y, z ]

Call this method before calling [ISurface::IMakeIsoCurves](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IMakeIsoCurves.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

[ISurface::IMakeIsoCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IMakeIsoCurve.html)

[ISurface::MakeIsoCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~MakeIsoCurve.html)

[ISurface::MakeIsoCurves Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~MakeIsoCurves.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP2, Revision Number 12.2