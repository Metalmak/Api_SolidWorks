<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~INewDrawing2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| INewDrawing2 Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : INewDrawing2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TemplateToUse*

*TemplateName*

*PaperSize*

*Width*

*Height*

Obsolete. Superseded by [ISldWorks::NewDocument](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~NewDocument.html) and [ISldWorks::INewDocument2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~INewDocument2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function INewDrawing2( _    ByVal TemplateToUse As System.Integer, _    ByVal TemplateName As System.String, _    ByVal PaperSize As System.Integer, _    ByVal Width As System.Double, _    ByVal Height As System.Double _ ) As DrawingDoc ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim TemplateToUse As System.Integer Dim TemplateName As System.String Dim PaperSize As System.Integer Dim Width As System.Double Dim Height As System.Double Dim value As DrawingDoc   value = instance.INewDrawing2(TemplateToUse, TemplateName, PaperSize, Width, Height) ``` | |

| C# |  |
| --- | --- |
| ``` DrawingDoc INewDrawing2(     System.int TemplateToUse,    System.string TemplateName,    System.int PaperSize,    System.double Width,    System.double Height ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` DrawingDoc^ INewDrawing2(  &   System.int TemplateToUse, &   System.String^ TemplateName, &   System.int PaperSize, &   System.double Width, &   System.double Height ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TemplateToUse*

*TemplateName*

*PaperSize*

*Width*

*Height*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::INewDrawing2.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)