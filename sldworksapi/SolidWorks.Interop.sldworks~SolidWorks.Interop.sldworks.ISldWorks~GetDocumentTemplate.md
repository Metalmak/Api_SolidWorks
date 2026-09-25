<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetDocumentTemplate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDocumentTemplate Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetDocumentTemplate Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Mode*
:   Document type as defined in swDocumentTypes\_e (see Remarks)

*TemplateName*
:   Name of custom template including full directory path

*PaperSize*
:   Size of paper as defined in swDwgPaperSizes\_e

*Width*
:   Width of paper; used only when paperSize is swDwgPapersUserDefined

*Height*
:   Height of paper; used only when paperSize is swDwgPapersUserDefined

Gets the name of document template that can be used in [ISldWorks::NewDocument](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~NewDocument.html) or [ISldWorks::INewDocument2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~INewDocument2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDocumentTemplate( _    ByVal Mode As System.Integer, _    ByVal TemplateName As System.String, _    ByVal PaperSize As System.Integer, _    ByVal Width As System.Double, _    ByVal Height As System.Double _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Mode As System.Integer Dim TemplateName As System.String Dim PaperSize As System.Integer Dim Width As System.Double Dim Height As System.Double Dim value As System.String   value = instance.GetDocumentTemplate(Mode, TemplateName, PaperSize, Width, Height) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetDocumentTemplate(     System.int Mode,    System.string TemplateName,    System.int PaperSize,    System.double Width,    System.double Height ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetDocumentTemplate(  &   System.int Mode, &   System.String^ TemplateName, &   System.int PaperSize, &   System.double Width, &   System.double Height ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Mode*
:   Document type as defined in swDocumentTypes\_e (see Remarks)

*TemplateName*
:   Name of custom template including full directory path

*PaperSize*
:   Size of paper as defined in swDwgPaperSizes\_e

*Width*
:   Width of paper; used only when paperSize is swDwgPapersUserDefined

*Height*
:   Height of paper; used only when paperSize is swDwgPapersUserDefined

#### Return Value

Name of the selected document template

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetDocumentTemplate.

# ![](dotnetimages/collapse.gif)Example

[Get Locations and Names of Document Templates (VBA)](Get_Locations_and_Names_of_Document_Templates_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| If type is... | Then... |
| swDocPART or swDocASSEMBLY | Remaining arguments are not used. |
| swDocDRAWING | Remaining arguments are used to determine which drawing template to use. |

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetTemplateSizes Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetTemplateSizes.html)

[ISldWorks::IGetTemplateSizes Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IGetTemplateSizes.html)

[ISldWorks::PreSelectDwgTemplateSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~PreSelectDwgTemplateSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP4, Revision Number 10.4