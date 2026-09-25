<!-- source: sw3dprinterapi/SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetScale.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS 3D Printer API Help | Send comments on this topic. |
| SetScale Method (ISw3DPrinter) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sw3dprinter Namespace](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter_namespace.html) > [ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html) : SetScale Method (ISw3DPrinter) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Scale*
:   Value by which to scale the document

Called when a user sets the value by which to scale the document in the Scale box on the 3D Printer tab.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetScale( _    ByVal Scale As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISw3DPrinter Dim Scale As System.Integer   instance.SetScale(Scale) ``` | |

| C# |  |
| --- | --- |
| ``` void SetScale(     System.int Scale ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetScale(  &   System.int Scale ) ``` | |

#### Parameters

*Scale*
:   Value by which to scale the document

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sw3DPrinter::SetScale.

# ![](dotnetimages/collapse.gif)See Also

####

[ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html)

[ISw3DPrinter Members](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter_members.html)

[ISw3DPrinter::GetScale Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetScale.html)

[ISw3DPrinter::GetScaleParametersForActiveDocument Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetScaleParametersForActiveDocument.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0