<!-- source: sw3dprinterapi/SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetEnvelopeOrigin.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS 3D Printer API Help | Send comments on this topic. |
| GetEnvelopeOrigin Method (ISw3DPrinter) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sw3dprinter Namespace](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter_namespace.html) > [ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html) : GetEnvelopeOrigin Method (ISw3DPrinter) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   x coordinate for starting location as defined in [swBuildEnvelopeStartingPoint\_e](SOLIDWORKS.Interop.sw3dprinter~SOLIDWORKS.Interop.sw3dprinter.swBuildEnvelopeStartingPoint_e.html)

*y*
:   y coordinate for starting location as defined in [swBuildEnvelopeStartingPoint\_e](SOLIDWORKS.Interop.sw3dprinter~SOLIDWORKS.Interop.sw3dprinter.swBuildEnvelopeStartingPoint_e.html)

*\_\_MIDL\_\_ISw3DPrinter0000*
:   z coordinate for starting location as defined in [swBuildEnvelopeStartingPoint\_e](SOLIDWORKS.Interop.sw3dprinter~SOLIDWORKS.Interop.sw3dprinter.swBuildEnvelopeStartingPoint_e.html)

Gets the default starting location for the item to be built in the build envelope, e.g. x-min, y-min, z-min.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetEnvelopeOrigin( _    ByRef X As swBuildEnvelopeStartingPoint_e, _    ByRef y As swBuildEnvelopeStartingPoint_e, _    ByRef __MIDL__ISw3DPrinter0000 As swBuildEnvelopeStartingPoint_e _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISw3DPrinter Dim X As swBuildEnvelopeStartingPoint_e Dim y As swBuildEnvelopeStartingPoint_e Dim __MIDL__ISw3DPrinter0000 As swBuildEnvelopeStartingPoint_e   instance.GetEnvelopeOrigin(X, y, __MIDL__ISw3DPrinter0000) ``` | |

| C# |  |
| --- | --- |
| ``` void GetEnvelopeOrigin(     out swBuildEnvelopeStartingPoint_e X,    out swBuildEnvelopeStartingPoint_e y,    out swBuildEnvelopeStartingPoint_e __MIDL__ISw3DPrinter0000 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetEnvelopeOrigin(  &   [Out] swBuildEnvelopeStartingPoint_e X, &   [Out] swBuildEnvelopeStartingPoint_e y, &   [Out] swBuildEnvelopeStartingPoint_e __MIDL__ISw3DPrinter0000 ) ``` | |

#### Parameters

*X*
:   x coordinate for starting location as defined in [swBuildEnvelopeStartingPoint\_e](SOLIDWORKS.Interop.sw3dprinter~SOLIDWORKS.Interop.sw3dprinter.swBuildEnvelopeStartingPoint_e.html)

*y*
:   y coordinate for starting location as defined in [swBuildEnvelopeStartingPoint\_e](SOLIDWORKS.Interop.sw3dprinter~SOLIDWORKS.Interop.sw3dprinter.swBuildEnvelopeStartingPoint_e.html)

*\_\_MIDL\_\_ISw3DPrinter0000*
:   z coordinate for starting location as defined in [swBuildEnvelopeStartingPoint\_e](SOLIDWORKS.Interop.sw3dprinter~SOLIDWORKS.Interop.sw3dprinter.swBuildEnvelopeStartingPoint_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sw3DPrinter::GetEnvelopeOrigin.

# ![](dotnetimages/collapse.gif)Remarks

In almost all cases, the printer's driver has set the Z origin to 0.0.

# ![](dotnetimages/collapse.gif)See Also

####

[ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html)

[ISw3DPrinter Members](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter_members.html)

[ISw3DPrinter::GetBuildEnvelope Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetBuildEnvelope.html)

[ISw3DPrinter::GetDefaultBuildOrientation Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetDefaultBuildOrientation.html)

[ISw3DPrinter::GetDefaultPrintQuality Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetDefaultPrintQuality.html)

[ISw3DPrinter::GetDialogConfiguration Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetDialogConfiguration.html)

[ISw3DPrinter::GetOutputOptions Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetOutputOptions.html)

[ISw3DPrinter::GetPrinterComment Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterComment.html)

[ISw3DPrinter::GetPrinterImageBitmap Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterImageBitmap.html)

[ISw3DPrinter::GetPrinterLocation Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterLocation.html)

[ISw3DPrinter::GetPrinterNames Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterNames.html)

[ISw3DPrinter::GetPrinterType Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterType.html)

[ISw3DPrinter::OnStartup Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~OnStartup.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0