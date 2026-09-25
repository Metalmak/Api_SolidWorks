<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetEllipseParams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetEllipseParams Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : IGetEllipseParams Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ParamArray*
:   * in-process, unmanaged C++: Pointer to an array of doubles (see **Remarks**)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

Gets the parameters for this elliptical curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetEllipseParams( _    ByRef ParamArray As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim ParamArray As System.Double   instance.IGetEllipseParams(ParamArray) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetEllipseParams(     ref System.double ParamArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetEllipseParams(  &   System.double% ParamArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ParamArray*
:   * in-process, unmanaged C++: Pointer to an array of doubles (see **Remarks**)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Use [ICurve::IsEllipse](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IsEllipse.html) to determine if a curve is an ellipse.

The return value is an array of doubles with the following format:

**[** *centerptX, centerptY, centerptZ, majorRad, majorAxisX, majorAxisY, majorAxisZ,
minorRad, minorAxisX, minorAxisY, minorAxisZ* **]**

where:

* *centerptX, centerptY, centerptZ*  = location of ellipse center* *majorRad*  = major radius* *majorAxisX*, *majorAxisY*, *majorAxisZ*  = major axis values* *minorRad*  = minor radius* *minorAxisX*, *minorAxisY*, *minorAxisZ* = minor axis values

You must pass an array of 11 doubles that has already been allocated. If you pass a NULL
pointer or the curve is not an ellipse, then SOLIDWORKS returns S\_false.

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::GetEllipseParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetEllipseParams.html)

[ICurve::Identity Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~Identity.html)