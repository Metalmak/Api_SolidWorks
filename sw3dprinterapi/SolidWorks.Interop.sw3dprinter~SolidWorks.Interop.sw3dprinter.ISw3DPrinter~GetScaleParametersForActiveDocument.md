<!-- source: sw3dprinterapi/SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetScaleParametersForActiveDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS 3D Printer API Help | Send comments on this topic. |
| GetScaleParametersForActiveDocument Method (ISw3DPrinter) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sw3dprinter Namespace](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter_namespace.html) > [ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html) : GetScaleParametersForActiveDocument Method (ISw3DPrinter) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*minimumScale*
:   Minimum scale value

*maximumScale*
:   Maximum scale value

*scaleIncrement*
:   Value by which to increment scale values

Gets the values by which the document can be scaled. The values appear in the Scale box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetScaleParametersForActiveDocument( _    ByRef minimumScale As System.Integer, _    ByRef maximumScale As System.Integer, _    ByRef scaleIncrement As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISw3DPrinter Dim minimumScale As System.Integer Dim maximumScale As System.Integer Dim scaleIncrement As System.Integer   instance.GetScaleParametersForActiveDocument(minimumScale, maximumScale, scaleIncrement) ``` | |

| C# |  |
| --- | --- |
| ``` void GetScaleParametersForActiveDocument(     out System.int minimumScale,    out System.int maximumScale,    out System.int scaleIncrement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetScaleParametersForActiveDocument(  &   [Out] System.int minimumScale, &   [Out] System.int maximumScale, &   [Out] System.int scaleIncrement ) ``` | |

#### Parameters

*minimumScale*
:   Minimum scale value

*maximumScale*
:   Maximum scale value

*scaleIncrement*
:   Value by which to increment scale values

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sw3DPrinter::GetScaleParametersForActiveDocument.

# ![](dotnetimages/collapse.gif)Remarks

These values appear in the Scale box.

This method is called when the user selects the vendor's printer.

When the user selects a printer from the list, that printer’s driver populates the Print dialog with default values. One of values is the scale parameters. For example, a printer might be able to scale between 10% and 300% in 5% increments. The printer's driver implements this method to return the minimum, maximum, and increment values, and SOLIDWORKS calls this method to return these values for that printer's driver.

# ![](dotnetimages/collapse.gif)See Also

####

[ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html)

[ISw3DPrinter Members](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter_members.html)

[ISw3DPrinter::GetScale Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetScale.html)

[ISw3DPrinter::SetScale Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetScale.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0