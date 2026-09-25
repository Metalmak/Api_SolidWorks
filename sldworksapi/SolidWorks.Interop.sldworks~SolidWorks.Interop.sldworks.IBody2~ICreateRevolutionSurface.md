<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateRevolutionSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateRevolutionSurface Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : ICreateRevolutionSurface Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ProfileCurve*
:   Profile curve (generatrix)

*AxisPoint*
:   Array of 3 doubles (x,y,z)

*AxisDirection*
:   Array of 3 doubles (x,y,z)

*ProfileEndPtParams*
:   Array of 2 doubles (uStart,uEnd) (see **Remarks**)

Creates a new surface of revolution.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateRevolutionSurface( _    ByVal ProfileCurve As Curve, _    ByVal AxisPoint As System.Object, _    ByVal AxisDirection As System.Object, _    ByVal ProfileEndPtParams As System.Object _ ) As Surface ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim ProfileCurve As Curve Dim AxisPoint As System.Object Dim AxisDirection As System.Object Dim ProfileEndPtParams As System.Object Dim value As Surface   value = instance.ICreateRevolutionSurface(ProfileCurve, AxisPoint, AxisDirection, ProfileEndPtParams) ``` | |

| C# |  |
| --- | --- |
| ``` Surface ICreateRevolutionSurface(     Curve ProfileCurve,    System.object AxisPoint,    System.object AxisDirection,    System.object ProfileEndPtParams ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Surface^ ICreateRevolutionSurface(  &   Curve^ ProfileCurve, &   System.Object^ AxisPoint, &   System.Object^ AxisDirection, &   System.Object^ ProfileEndPtParams ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ProfileCurve*
:   Profile curve (generatrix)

*AxisPoint*
:   Array of 3 doubles (x,y,z)

*AxisDirection*
:   Array of 3 doubles (x,y,z)

*ProfileEndPtParams*
:   Array of 2 doubles (uStart,uEnd) (see **Remarks**)

#### Return Value

Pointer to a new [surface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface.html) of revolution

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::ICreateRevolutionSurface.

# ![](dotnetimages/collapse.gif)Remarks

You can use this method with:

* A set of related functions that construct a body from trimmed surfaces.* Trimming curve creation routines (for example, [ISurface::IAddTrimmingLoop2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IAddTrimmingLoop2.html)) to construct a trimmed surface of revolution.

If you pass ProfileEndPtParams to this method, the surface is trimmed in the axial direction; otherwise, it is infinite. SOLIDWORKS closes the surface periodic ( period [0,2PI]) in the direction of revolution. The ProfileEndPtParams parameters indicate to SOLIDWORKS which part of the curve to spin. These parameters are used only when the profile curve intersects the revolve axis. You must pass the parameters in ascending order. SOLIDWORKS extends the curve from the given parameter range to meet the revolve axis and spins this portion of curve.

You can also pass an empty VARIANT object to ProfileEndPtParams; it cannot be NULL. You must define a variable of type VARIANT.

Any existing object created by this method is destroyed if you call this method again.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::CreateRevolutionSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateRevolutionSurface.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0