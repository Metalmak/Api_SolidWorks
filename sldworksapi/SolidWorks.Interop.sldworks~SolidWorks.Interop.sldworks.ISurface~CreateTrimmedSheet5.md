<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~CreateTrimmedSheet5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateTrimmedSheet5 Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : CreateTrimmedSheet5 Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Curves*
:   Array of [curves](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) that represent the boundary of the trimmed sheet (see **Remarks**)

*PreserveAnalyticCurves*
:   True to preserve analytic curves, false to store all trimming curves as SP-curves

*Tolerance*
:   Tolerance for gaps between edges (see **Remarks**)

Creates a trimmed sheet body from this surface.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateTrimmedSheet5( _    ByVal Curves As System.Object, _    ByVal PreserveAnalyticCurves As System.Boolean, _    ByVal Tolerance As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim Curves As System.Object Dim PreserveAnalyticCurves As System.Boolean Dim Tolerance As System.Double Dim value As System.Object   value = instance.CreateTrimmedSheet5(Curves, PreserveAnalyticCurves, Tolerance) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateTrimmedSheet5(     System.object Curves,    System.bool PreserveAnalyticCurves,    System.double Tolerance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateTrimmedSheet5(  &   System.Object^ Curves, &   System.bool PreserveAnalyticCurves, &   System.double Tolerance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Curves*
:   Array of [curves](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) that represent the boundary of the trimmed sheet (see **Remarks**)

*PreserveAnalyticCurves*
:   True to preserve analytic curves, false to store all trimming curves as SP-curves

*Tolerance*
:   Tolerance for gaps between edges (see **Remarks**)

#### Return Value

Temporary sheet [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::CreateTrimmedSheet5.

# ![](dotnetimages/collapse.gif)Example

'VBA

'===========================================
'Preconditions:
'1. Open a new part.
'2. Run the macro to the Stop.
'3. Press F5 to create the imported feature.
'
'Postconditions:
'1. Creates a temporary body and displays it.
'2. Uses the temporary body to create **Surface-Imported1**
'   in the FeatureManager design tree.
'===========================================

Const RADIUS As Double = 0.01

Dim swApp As SldWorks.SldWorks
Dim swPart As SldWorks.PartDoc
Dim swSurf As SldWorks.Surface
Dim swBody As SldWorks.Body2
Dim swFeat As SldWorks.Feature
Dim swModeler As SldWorks.Modeler

Option Explicit

Sub main()

    Set swApp = Application.SldWorks
    Set swPart = swApp.ActiveDoc

    Set swModeler = swApp.GetModeler

    Dim dCenter(2) As Double
    dCenter(0) = 0: dCenter(1) = 0: dCenter(2) = 0

    Dim dAxis(2) As Double
    dAxis(0) = 0: dAxis(1) = 0: dAxis(2) = 1

    Dim dRef(2) As Double
    dRef(0) = 1: dRef(1) = 0: dRef(2) = 0

    Set swSurf = swModeler.CreateSphericalSurface2(dCenter, dAxis, dRef, RADIUS)

    ' No trimming curves are required, so pass one Nothing in the Curves parameter array
    ' of ISurface::CreateTrimmedSheet5
    Dim ZeroTrimmingCurves(0 To 0) As SldWorks.Curve
    Set ZeroTrimmingCurves(0) = Nothing
    Set swBody = swSurf.**CreateTrimmedSheet5**(ZeroTrimmingCurves, True, 0.00001)

    swBody.**Display3** swPart, RGB(255, 255, 0), swTempBodySelectOptions\_e.swTempBodySelectable

    Stop

    Set swFeat = swPart.**CreateFeatureFromBody3**(swBody, False, swCreateFeatureBodyOpts\_e.swCreateFeatureBodyCheck + swCreateFeatureBodyOpts\_e.swCreateFeatureBodySimplify)

End Sub

# ![](dotnetimages/collapse.gif)Remarks

The Curves array contains all of the curves required to add the appropriate trimming loops to the surface. A null or Nothing entry in the array represents the separation between loops.

The trimming curves supplied are assumed to lie on the surface. If the curves are 2D curves, then they should be created using this surface.

If your application is creating a trimmed sheet body from a periodic surface without trimming curves, then the Curves array should contain only one entry: null or Nothing.

Tolerance sets the edge precision in PK\_SURF\_make\_sheet\_trimmed. The default parasolid tolerance is 0.00001. This parameter allows you to specify a looser tolerance for gaps between edges.

Before calling this method, trim the curves created by [IModeler::CreateArc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~CreateArc.html) and [IModeler::CreateLine](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~CreateLine.html) by calling [ICurve::CreateTrimmedCurve2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~CreateTrimmedCurve2.html). Elliptical curves created by [IModeler::CreateEllipse](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~CreateEllipse.html) do not need to be trimmed before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 SP4, Revision Number 25.4