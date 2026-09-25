<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IGetTemplateSizes.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetTemplateSizes Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : IGetTemplateSizes Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Name of template with full directory path

*PaperSize*
:   Paper size as defined in swDwgPaperSizes\_e

*Width*
:   Custom paper width if PaperSize is set to swDwgPapersUserDefined

*Height*
:   Custom paper height if PaperSize is set to swDwgPapersUserDefined

Gets the sheet properties from a template document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetTemplateSizes( _    ByVal FileName As System.String, _    ByRef PaperSize As System.Integer, _    ByRef Width As System.Double, _    ByRef Height As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FileName As System.String Dim PaperSize As System.Integer Dim Width As System.Double Dim Height As System.Double Dim value As System.Boolean   value = instance.IGetTemplateSizes(FileName, PaperSize, Width, Height) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IGetTemplateSizes(     System.string FileName,    out System.int PaperSize,    out System.double Width,    out System.double Height ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IGetTemplateSizes(  &   System.String^ FileName, &   [Out] System.int PaperSize, &   [Out] System.double Width, &   [Out] System.double Height ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Name of template with full directory path

*PaperSize*
:   Paper size as defined in swDwgPaperSizes\_e

*Width*
:   Custom paper width if PaperSize is set to swDwgPapersUserDefined

*Height*
:   Custom paper height if PaperSize is set to swDwgPapersUserDefined

#### Return Value

True if the operation is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::IGetTemplateSizes.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetTemplateSizes Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetTemplateSizes.html)

[ISldWorks::GetDocumentTemplate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetDocumentTemplate.html)

[ISldWorks::PreSelectDwgTemplateSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~PreSelectDwgTemplateSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0