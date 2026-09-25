<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~NewDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| NewDocument Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : NewDocument Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TemplateName*
:   Fully qualified path and name of the template to use for creating the new document

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
| ``` Function NewDocument( _    ByVal TemplateName As System.String, _    ByVal PaperSize As System.Integer, _    ByVal Width As System.Double, _    ByVal Height As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim TemplateName As System.String Dim PaperSize As System.Integer Dim Width As System.Double Dim Height As System.Double Dim value As System.Object   value = instance.NewDocument(TemplateName, PaperSize, Width, Height) ``` | |

| C# |  |
| --- | --- |
| ``` System.object NewDocument(     System.string TemplateName,    System.int PaperSize,    System.double Width,    System.double Height ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ NewDocument(  &   System.String^ TemplateName, &   System.int PaperSize, &   System.double Width, &   System.double Height ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TemplateName*
:   Fully qualified path and name of the template to use for creating the new document

*PaperSize*
:   Size of paper as defined in swDwgPaperSizes\_e

*Width*
:   Width of paper; used only when PaperSize is swDwgPapersUserDefined

*Height*
:   Height of paper; used only when PaperSize is swDwgPapersUserDefined

#### Return Value

Newly created [document](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) or NULL if the operation fails

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::NewDocument.

# ![](dotnetimages/collapse.gif)Example

[Combine Assembly Components Into Part (VBA)](Combine_Assembly_Components_into_Part_Example_VB.htm)

[Dimension Edge in Drawing (VBA)](Dimension_Edge_in_Drawing_Example_VB.htm)

[Insert Conic Curve (C#)](Insert_Conic_Curve_Example_CSharp.htm)

[Insert Conic Curve (VB.NET)](Insert_Conic_Curve_Example_VBNET.htm)

[Insert Conic Curve (VBA)](Insert_Conic_Curve_Example_VB.htm)

[Insert Model Annotations (C#)](Insert_Model_Annotations_Example_CSharp.htm)

[Insert Model Annotations (VB.NET)](Insert_Model_Annotations_Example_VBNET.htm)

[Insert Model Annotations (VBA)](Insert_Model_Annotations_Example_VB.htm)

[Process Body (C#)](Process_Body_Example_CSharp.htm)

[Process Body (VB.NET)](Process_Body_Example_VBNET.htm)

[Process Body (VBA)](Process_Body_Example_VB.htm)

[Fill Holes in Part (C#)](Fill_Holes_in_Part_Example_CSharp.htm)

[Fill Holes in Part (VB.NET)](Fill_Holes_in_Part_Example_VBNET.htm)

[Fill Holes in Part (VBA)](Fill_Holes_in_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To get the default template filename, use [ISldWorks::GetUserPreferenceStringValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetUserPreferenceStringValue.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetDocumentTemplate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetDocumentTemplate.html)

[ISldWorks::INewDocument2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~INewDocument2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0