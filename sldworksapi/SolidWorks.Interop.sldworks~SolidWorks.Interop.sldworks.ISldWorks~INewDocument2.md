<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~INewDocument2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| INewDocument2 Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : INewDocument2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TemplateName*
:   Name of the template to use for creating the new document

*PaperSize*
:   Size of paper as defined in swDwgPaperSizes\_e

*Width*
:   Width of paper; used only when PaperSize is swDwgPapersUserDefined

*Height*
:   Height of paper; used only when PaperSize is swDwgPapersUserDefined

Creates a new document based on the specified template.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function INewDocument2( _    ByVal TemplateName As System.String, _    ByVal PaperSize As System.Integer, _    ByVal Width As System.Double, _    ByVal Height As System.Double _ ) As ModelDoc2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim TemplateName As System.String Dim PaperSize As System.Integer Dim Width As System.Double Dim Height As System.Double Dim value As ModelDoc2   value = instance.INewDocument2(TemplateName, PaperSize, Width, Height) ``` | |

| C# |  |
| --- | --- |
| ``` ModelDoc2 INewDocument2(     System.string TemplateName,    System.int PaperSize,    System.double Width,    System.double Height ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` ModelDoc2^ INewDocument2(  &   System.String^ TemplateName, &   System.int PaperSize, &   System.double Width, &   System.double Height ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TemplateName*
:   Name of the template to use for creating the new document

*PaperSize*
:   Size of paper as defined in swDwgPaperSizes\_e

*Width*
:   Width of paper; used only when PaperSize is swDwgPapersUserDefined

*Height*
:   Height of paper; used only when PaperSize is swDwgPapersUserDefined

#### Return Value

Newly created [document](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) or NULL if the operation fails

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::INewDocument2.

# ![](dotnetimages/collapse.gif)Example

[Access Assembly (C++)](Access_Assembly_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

To get the default template filename, use [ISldWorks::GetUserPreferenceStringValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetUserPreferenceStringValue.html):

* for parts: swDefaultTemplatePart

  * for assemblies: swDefaultTemplateAssembly

    * for drawings: swDefaultTemplateDrawing

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetDocumentTemplate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetDocumentTemplate.html)

[ISldWorks::NewDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~NewDocument.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0