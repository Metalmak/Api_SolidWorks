<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IGetBSurfParamsSize3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetBSurfParamsSize3 Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : IGetBSurfParamsSize3 Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WantCubic*
:   True for surface to be a cubic, false for not

*WantNonRational*
:   True if non-rational is needed, false if not; specifying true converts any surface type to a non-rational Bsurface; if you specify true, then you should only use this method for surfaces that are Bsurface or blend surface; otherwise, the underlying call is not made and the values returned from this are not initialized or contain the values from the last call

*Range*
:   Array of 4 doubles describing the U,V Range

*Tolerance*
:   Tolerance, in meters, between the approximated b-spline surface and the underlying surface; the default value is 0.01 and should generally be reduced to the tolerance desired

*Sense*
:   Approximated b-spline surface is not always in the same direction as the original surface; if sense is true, then the underlying surface and the b-spline surface are in the same direction

Gets the allocation size necessary for Bsurface parameter data retrieval in a subsequent call to [ISurface::IGetBSurfParams](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IGetBSurfParams.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetBSurfParamsSize3( _    ByVal WantCubic As System.Boolean, _    ByVal WantNonRational As System.Boolean, _    ByRef Range As System.Double, _    ByVal Tolerance As System.Double, _    ByRef Sense As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim WantCubic As System.Boolean Dim WantNonRational As System.Boolean Dim Range As System.Double Dim Tolerance As System.Double Dim Sense As System.Boolean Dim value As System.Integer   value = instance.IGetBSurfParamsSize3(WantCubic, WantNonRational, Range, Tolerance, Sense) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetBSurfParamsSize3(     System.bool WantCubic,    System.bool WantNonRational,    ref System.double Range,    System.double Tolerance,    out System.bool Sense ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetBSurfParamsSize3(  &   System.bool WantCubic, &   System.bool WantNonRational, &   System.double% Range, &   System.double Tolerance, &   [Out] System.bool Sense ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WantCubic*
:   True for surface to be a cubic, false for not

*WantNonRational*
:   True if non-rational is needed, false if not; specifying true converts any surface type to a non-rational Bsurface; if you specify true, then you should only use this method for surfaces that are Bsurface or blend surface; otherwise, the underlying call is not made and the values returned from this are not initialized or contain the values from the last call

*Range*
:   Array of 4 doubles describing the U,V Range

*Tolerance*
:   Tolerance, in meters, between the approximated b-spline surface and the underlying surface; the default value is 0.01 and should generally be reduced to the tolerance desired

*Sense*
:   Approximated b-spline surface is not always in the same direction as the original surface; if sense is true, then the underlying surface and the b-spline surface are in the same direction

#### Return Value

Size of the data set

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::IGetBSurfParamsSize3.

# ![](dotnetimages/collapse.gif)Remarks

Range contains the following values that can be obtained using [ISurface::Parameterization](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~Parameterization.html) or [ISurface::IParameterization](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IParameterization.html):

* Range[0] & Range[2] are the lower bounds of the U & V surface parameters respectively.

  * Range[1] & Range[3] are the upper bounds of the U & V surface parameters respectively.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 SP3, Revision Number 8.3