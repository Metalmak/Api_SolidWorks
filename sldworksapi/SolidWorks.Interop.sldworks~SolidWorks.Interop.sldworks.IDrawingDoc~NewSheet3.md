<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~NewSheet3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| NewSheet3 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : NewSheet3 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Name to be given to the new drawing sheet

*PaperSize*
:   Size of paper if using swDwgTemplateNone as defined in swDwgPaperSizes\_e

*TemplateIn*
:   Template as defined in swDwgTemplates\_e

*Scale1*
:   Scale numerator

*Scale2*
:   Scale denominator

*FirstAngle*
:   True for first angle projection, false otherwise

*TemplateName*
:   Name of custom template with full directory path if TemplateIn is set to swDwgTemplateCustom

*Width*
:   Paper width if TemplateIn is set to swDwgTemplateNone or swDwgPapersUserDefined

*Height*
:   Paper height if TemplateIn is set to swDwgTemplateNone or swDwgPapersUserDefined

*PropertyViewName*
:   Name of the drawing view containing the model custom property values

Obsolete. Superseded by [IDrawingDoc::NewSheet4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~NewSheet4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function NewSheet3( _    ByVal Name As System.String, _    ByVal PaperSize As System.Integer, _    ByVal TemplateIn As System.Integer, _    ByVal Scale1 As System.Double, _    ByVal Scale2 As System.Double, _    ByVal FirstAngle As System.Boolean, _    ByVal TemplateName As System.String, _    ByVal Width As System.Double, _    ByVal Height As System.Double, _    ByVal PropertyViewName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Name As System.String Dim PaperSize As System.Integer Dim TemplateIn As System.Integer Dim Scale1 As System.Double Dim Scale2 As System.Double Dim FirstAngle As System.Boolean Dim TemplateName As System.String Dim Width As System.Double Dim Height As System.Double Dim PropertyViewName As System.String Dim value As System.Boolean   value = instance.NewSheet3(Name, PaperSize, TemplateIn, Scale1, Scale2, FirstAngle, TemplateName, Width, Height, PropertyViewName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool NewSheet3(     System.string Name,    System.int PaperSize,    System.int TemplateIn,    System.double Scale1,    System.double Scale2,    System.bool FirstAngle,    System.string TemplateName,    System.double Width,    System.double Height,    System.string PropertyViewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool NewSheet3(  &   System.String^ Name, &   System.int PaperSize, &   System.int TemplateIn, &   System.double Scale1, &   System.double Scale2, &   System.bool FirstAngle, &   System.String^ TemplateName, &   System.double Width, &   System.double Height, &   System.String^ PropertyViewName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name to be given to the new drawing sheet

*PaperSize*
:   Size of paper if using swDwgTemplateNone as defined in swDwgPaperSizes\_e

*TemplateIn*
:   Template as defined in swDwgTemplates\_e

*Scale1*
:   Scale numerator

*Scale2*
:   Scale denominator

*FirstAngle*
:   True for first angle projection, false otherwise

*TemplateName*
:   Name of custom template with full directory path if TemplateIn is set to swDwgTemplateCustom

*Width*
:   Paper width if TemplateIn is set to swDwgTemplateNone or swDwgPapersUserDefined

*Height*
:   Paper height if TemplateIn is set to swDwgTemplateNone or swDwgPapersUserDefined

*PropertyViewName*
:   Name of the drawing view containing the model custom property values

#### Return Value

True if drawing sheet creation was successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::NewSheet3.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::ActivateSheet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ActivateSheet.html)

[IDrawingDoc::EditSheet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~EditSheet.html)

[IDrawingDoc::GetCurrentSheet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~GetCurrentSheet.html)

[IDrawingDoc::GetSheetCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~GetSheetCount.html)

[IDrawingDoc::GetSheetNames Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~GetSheetNames.html)

[IDrawingDoc::IGetCurrentSheet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IGetCurrentSheet.html)

[IDrawingDoc::IGetSheetNames Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IGetSheetNames.html)

[IDrawingDoc::IReorderSheets Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IReorderSheets.html)

[IDrawingDoc::ReorderSheets Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ReorderSheets.html)

[IDrawingDoc::SetupSheet4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~SetupSheet4.html)

[IDrawingDoc::SheetNext Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~SheetNext.html)

[IDrawingDoc::SheetPrevious Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~SheetPrevious.html)

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)