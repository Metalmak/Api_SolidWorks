<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ExtentCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ExtentCurve Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : ExtentCurve Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AtStart*
:   True to extend b-spline curve from start point, false to extend b-spline curve from end point

*Length*
:   Length by which to extend b-spline curve

*LinearExt*
:   True if the extension is linear, false if not

Extends a b-spline curve by the specified length.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ExtentCurve( _    ByVal AtStart As System.Boolean, _    ByVal Length As System.Double, _    ByVal LinearExt As System.Boolean _ ) As Curve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim AtStart As System.Boolean Dim Length As System.Double Dim LinearExt As System.Boolean Dim value As Curve   value = instance.ExtentCurve(AtStart, Length, LinearExt) ``` | |

| C# |  |
| --- | --- |
| ``` Curve ExtentCurve(     System.bool AtStart,    System.double Length,    System.bool LinearExt ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Curve^ ExtentCurve(  &   System.bool AtStart, &   System.double Length, &   System.bool LinearExt ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AtStart*
:   True to extend b-spline curve from start point, false to extend b-spline curve from end point

*Length*
:   Length by which to extend b-spline curve

*LinearExt*
:   True if the extension is linear, false if not

#### Return Value

Pointer to newly extended [ICurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::ExtentCurve.

# ![](dotnetimages/collapse.gif)Remarks

This method only affects b-spline curves. For all other types of curves, this method does nothing.

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::CreateTrimmedCurve2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~CreateTrimmedCurve2.html)

[ICurve::IConvertPcurveToBcurveSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IConvertPcurveToBcurveSize.html)

[ICurve::IJoinCurves Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IJoinCurves.html)

[ICurve::JoinCurves Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~JoinCurves.html)

[ICurve::MakeBsplineCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~MakeBsplineCurve.html)

[ICurve::ReverseCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ReverseCurve.html)

[ICurve::SimplifyBCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~SimplifyBCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0