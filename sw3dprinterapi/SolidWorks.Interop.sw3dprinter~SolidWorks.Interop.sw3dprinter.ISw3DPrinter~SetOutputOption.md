<!-- source: sw3dprinterapi/SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetOutputOption.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS 3D Printer API Help | Send comments on this topic. |
| SetOutputOption Method (ISw3DPrinter) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sw3dprinter Namespace](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter_namespace.html) > [ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html) : SetOutputOption Method (ISw3DPrinter) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OutputOption*
:   Selection that specifies how to create the rapid prototype

Called when a user specifies how to create the rapid prototype by making a selection in the **Output** box on the 3D Printer tab.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetOutputOption( _    ByVal OutputOption As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISw3DPrinter Dim OutputOption As System.String   instance.SetOutputOption(OutputOption) ``` | |

| C# |  |
| --- | --- |
| ``` void SetOutputOption(     System.string OutputOption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetOutputOption(  &   System.String^ OutputOption ) ``` | |

#### Parameters

*OutputOption*
:   Selection that specifies how to create the rapid prototype

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sw3DPrinter::SetOutputOption.

# ![](dotnetimages/collapse.gif)See Also

####

[ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html)

[ISw3DPrinter Members](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter_members.html)

[ISw3DPrinter::GetOutputOption Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetOutputOption.html)

[ISw3DPrinter::GetOutputOptions Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetOutputOptions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0