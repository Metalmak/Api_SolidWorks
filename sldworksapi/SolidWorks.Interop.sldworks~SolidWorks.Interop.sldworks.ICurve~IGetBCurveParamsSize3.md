<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetBCurveParamsSize3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetBCurveParamsSize3 Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : IGetBCurveParamsSize3 Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WantCubicIn*
:   True for cubic curves, false if not

*WantNRational*
:   True for non-rational curves, false if not

*ForceNonPeriodic*
:   True converts the curve to nonperiodic and returns parameters, false does not

Gets the b-curve size.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetBCurveParamsSize3( _    ByVal WantCubicIn As System.Boolean, _    ByVal WantNRational As System.Boolean, _    ByVal ForceNonPeriodic As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim WantCubicIn As System.Boolean Dim WantNRational As System.Boolean Dim ForceNonPeriodic As System.Boolean Dim value As System.Integer   value = instance.IGetBCurveParamsSize3(WantCubicIn, WantNRational, ForceNonPeriodic) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetBCurveParamsSize3(     System.bool WantCubicIn,    System.bool WantNRational,    System.bool ForceNonPeriodic ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetBCurveParamsSize3(  &   System.bool WantCubicIn, &   System.bool WantNRational, &   System.bool ForceNonPeriodic ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WantCubicIn*
:   True for cubic curves, false if not

*WantNRational*
:   True for non-rational curves, false if not

*ForceNonPeriodic*
:   True converts the curve to nonperiodic and returns parameters, false does not

#### Return Value

Size of the data set returned by [ICurve::IGetBCurveParams3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IGetBCurveParams3.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::IGetBCurveParamsSize3.

# ![](dotnetimages/collapse.gif)Remarks

Use this method to control the type of information returned in the subsequent call to [ICurve::IGetBCurveParams3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IGetBCurveParams3.html).

To control the accuracy of the curve data, see [IModeler::SetToleranceValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~SetToleranceValue.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::GetBCurveParams3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetBCurveParams3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP5, Revision Number 15.5