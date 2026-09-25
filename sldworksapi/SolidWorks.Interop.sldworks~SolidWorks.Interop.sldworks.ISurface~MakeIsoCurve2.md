<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~MakeIsoCurve2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MakeIsoCurve2 Method (ISurface) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : MakeIsoCurve2 Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UorV*
:   True to specify the surface function's v parameter in UvValue, false to specify its u parameter

*UvValue*
:   | If UorV is... | Then UvValue is the surface function's... |
    | --- | --- |
    | True | V parameter |
    | False | U parameter |

Creates an untrimmed curve on a surface using the specified u or v surface function parameter.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MakeIsoCurve2( _    ByVal UorV As System.Boolean, _    ByRef UvValue As System.Double _ ) As Curve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim UorV As System.Boolean Dim UvValue As System.Double Dim value As Curve   value = instance.MakeIsoCurve2(UorV, UvValue) ``` | |

| C# |  |
| --- | --- |
| ``` Curve MakeIsoCurve2(     System.bool UorV,    out System.double UvValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Curve^ MakeIsoCurve2(  &   System.bool UorV, &   [Out] System.double UvValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UorV*
:   True to specify the surface function's v parameter in UvValue, false to specify its u parameter

*UvValue*
:   | If UorV is... | Then UvValue is the surface function's... |
    | --- | --- |
    | True | V parameter |
    | False | U parameter |

#### Return Value

[Curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::MakeIsoCurve2.

# ![](dotnetimages/collapse.gif)Example

[Create Trimmed Curve (VBA)](Return_Untrimmed_Curve_Example_VB.htm)

[Create Trimmed Curve (VB.NET)](Return_Untrimmed_Curve_Example_VBNET.htm)

[Create Trimmed Curve (C#)](Return_Untrimmed_Curve_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes the now obsolete ISurface::MakeIsoCurve by normalizing UvValue when it exceeds a specific value.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

[ISurface::MakeIsoCurves Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~MakeIsoCurves.html)

[ISurface::IMakeIsoCurves Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IMakeIsoCurves.html)

[ISurface::IGetMakeIsoCurvesCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IGetMakeIsoCurvesCount.html)

[ISurface::IMakeIsoCurve Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IMakeIsoCurve.html)

[ICurve::CreateTrimmedCurve2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~CreateTrimmedCurve2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 SP05, Revision Number 21.5