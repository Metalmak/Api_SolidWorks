<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~GetBSurfParams3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBSurfParams3 Method (ISurface) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : GetBSurfParams3 Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WantCubic*
:   True if cubic is needed, false if not; specifying true converts any surface to a cubic B-spline surface

*WantNonRational*
:   True if non-rational is needed, false if not; specifying true converts any surface to a non-rational B-spline surface; if you specify true, then you should only use this method for surfaces that are of B-spline or blend type; otherwise, the underlying call is not made and the values returned from this are not initialized, or they contain the values from the last call

*VP0*
:   [ISurfaceParameterizationData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurfaceParameterizationData.html)

*Tolerance*
:   Tolerance, in meters, between the approximated B-spline surface and the underlying surface; the default value is 0.01 and should generally be reduced to the tolerance desired

*Sense*
:   Approximated B-spline surface is not always in the same direction as the original surface; if Sense is true, then the underlying surface and the B-spline surface are in the same direction

Gets the parameterization data for a B-spline surface.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBSurfParams3( _    ByVal WantCubic As System.Boolean, _    ByVal WantNonRational As System.Boolean, _    ByVal VP0 As System.Object, _    ByVal Tolerance As System.Double, _    ByRef Sense As System.Boolean _ ) As BSurfParamData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim WantCubic As System.Boolean Dim WantNonRational As System.Boolean Dim VP0 As System.Object Dim Tolerance As System.Double Dim Sense As System.Boolean Dim value As BSurfParamData   value = instance.GetBSurfParams3(WantCubic, WantNonRational, VP0, Tolerance, Sense) ``` | |

| C# |  |
| --- | --- |
| ``` BSurfParamData GetBSurfParams3(     System.bool WantCubic,    System.bool WantNonRational,    System.object VP0,    System.double Tolerance,    out System.bool Sense ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` BSurfParamData^ GetBSurfParams3(  &   System.bool WantCubic, &   System.bool WantNonRational, &   System.Object^ VP0, &   System.double Tolerance, &   [Out] System.bool Sense ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WantCubic*
:   True if cubic is needed, false if not; specifying true converts any surface to a cubic B-spline surface

*WantNonRational*
:   True if non-rational is needed, false if not; specifying true converts any surface to a non-rational B-spline surface; if you specify true, then you should only use this method for surfaces that are of B-spline or blend type; otherwise, the underlying call is not made and the values returned from this are not initialized, or they contain the values from the last call

*VP0*
:   [ISurfaceParameterizationData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurfaceParameterizationData.html)

*Tolerance*
:   Tolerance, in meters, between the approximated B-spline surface and the underlying surface; the default value is 0.01 and should generally be reduced to the tolerance desired

*Sense*
:   Approximated B-spline surface is not always in the same direction as the original surface; if Sense is true, then the underlying surface and the B-spline surface are in the same direction

#### Return Value

An [IBSurfParamData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBSurfParamData.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::GetBSurfParams3.

# ![](dotnetimages/collapse.gif)Example

[Get B-Spline Surface Parameterization Data (C#)](Get_B-Spline_Surface_Parameterization_Data_Example_CSharp.htm)

[Get B-Spline Surface Parameterization Data (VB.NET)](Get_B-Spline_Surface_Parameterization_Data_Example_VBNET.htm)

[Get B-Spline Surface Parameterization Data (VBA)](Get_B-Spline_Surface_Parameterization_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ISurface:Parameterization2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~Parameterization2.html) to populate VP0.

If you want to use the B-spline surface in combination with its trim curves, you should use the [IFace2::GetTrimCurves2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetTrimCurves2.html) method to extract both the trim curves and the B-spline surface. The [IFace2::GetTrimCurves2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetTrimCurves2.html) method provides much better alignment of the trim curves with the B-spline surface, because they are both generated at the same time.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

[ISurface::IGetBSurfParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IGetBSurfParams.html)

[ISurface::IGetBSurfParamsSize3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IGetBSurfParamsSize3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0