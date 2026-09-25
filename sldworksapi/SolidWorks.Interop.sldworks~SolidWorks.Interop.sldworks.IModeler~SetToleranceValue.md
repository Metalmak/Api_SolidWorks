<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~SetToleranceValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetToleranceValue Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : SetToleranceValue Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ToleranceID*
:   Type of tolerance you want to set as defined in swTolerances\_e

*NewToleranceValue*
:   New tolerance value in meters for the specified tolerance type

Sets tolerances governing geometry output.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetToleranceValue( _    ByVal ToleranceID As System.Integer, _    ByVal NewToleranceValue As System.Double _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim ToleranceID As System.Integer Dim NewToleranceValue As System.Double Dim value As System.Double   value = instance.SetToleranceValue(ToleranceID, NewToleranceValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.double SetToleranceValue(     System.int ToleranceID,    System.double NewToleranceValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double SetToleranceValue(  &   System.int ToleranceID, &   System.double NewToleranceValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ToleranceID*
:   Type of tolerance you want to set as defined in swTolerances\_e

*NewToleranceValue*
:   New tolerance value in meters for the specified tolerance type

#### Return Value

Original value of the specified tolerance type

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::SetToleranceValue.

# ![](dotnetimages/collapse.gif)Remarks

The default tolerance setting for 3D geometry output is 0.01 meters, while 2D geometry uses a 1e-4 dimensionless tolerance value. If your 3D trim curves are coming out too far from the surfaces they are trimming or are not close to the 2D trim curves, then you might want to tighten the tolerance. Set the tolerances before any extraction of geometry.

The tolerance values can be reset by other AddIns such as IGES. Make sure that they are set to your values when you need them. The tolerance settings only affect other AddIn applications. However, you should be careful to reset the tolerances so that other AddIn applications are not affected by your choice of tolerance.

The swUVCurveOutputTol tolerance is used during the extraction of UV (SP) trim curves. The [IFace2::GetTrimCurves2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetTrimCurves2.html) method is affected by this setting. This tolerance value represents a fraction of the characteristic small dimension of a face (the tolerance is dimensionless). For example, if you set the swUVCurveOutputTol tolerance value to 3e-6 and the smallest dimension of the face is 0.4 meters, then the largest deviation of the trim curve will be:

(0.4 x 3e-6) meters

For reference, the SOLIDWORKS IGES processor lets you control the swUVCurveOutputTol tolerance setting in the user preferences area. The normal setting under IGES uses a tolerance of 1e-4, while the high setting changes this tolerance to 3e-6. The IGES setting does not affect your application. Higher tolerance settings can increase processing time and the size of any output results.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::GetToleranceValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~GetToleranceValue.html)

[IModeler::UnsetTolerances Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~UnsetTolerances.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 SP3, Revision Number 8.3