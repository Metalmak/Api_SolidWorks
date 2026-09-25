<!-- source: sw3dprinterapi/SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedSurfaceArea.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS 3D Printer API Help | Send comments on this topic. |
| GetCalculatedSurfaceArea Method (ISw3DPrinter) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sw3dprinter Namespace](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter_namespace.html) > [ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html) : GetCalculatedSurfaceArea Method (ISw3DPrinter) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the calculated surface area of the current document in current document units, taking into account scale and other parameters.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCalculatedSurfaceArea() As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISw3DPrinter Dim value As System.String   value = instance.GetCalculatedSurfaceArea() ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetCalculatedSurfaceArea() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetCalculatedSurfaceArea(); ``` | |

#### Return Value

Calculated surface area of the current document in current document units

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sw3DPrinter::GetCalculatedSurfaceArea.

# ![](dotnetimages/collapse.gif)See Also

####

[ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html)

[ISw3DPrinter Members](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter_members.html)

[ISw3DPrinter::GetCalculatedBoundingVolume Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedBoundingVolume.html)

[ISw3DPrinter::GetCalculatedBuildTime Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedBuildTime.html)

[ISw3DPrinter::GetCalculatedCost Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedCost.html)

[ISw3DPrinter::GetCalculatedVolume Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedVolume.html)

[ISw3DPrinter::OnUpdateStatistics Method](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~OnUpdateStatistics.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0