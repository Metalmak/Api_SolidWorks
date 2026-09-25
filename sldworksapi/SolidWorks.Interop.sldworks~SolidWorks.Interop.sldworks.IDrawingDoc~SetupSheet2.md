<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~SetupSheet2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetupSheet2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : SetupSheet2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*

*PaperSize*

*TemplateIn*

*Scale1*

*Scale2*

*SkPointsFlag*

Obsolete. Superseded by [IDrawingDoc::SetupSheet4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~SetupSheet4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetupSheet2( _    ByVal Name As System.String, _    ByVal PaperSize As System.Short, _    ByVal TemplateIn As System.Short, _    ByVal Scale1 As System.Double, _    ByVal Scale2 As System.Double, _    ByVal SkPointsFlag As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Name As System.String Dim PaperSize As System.Short Dim TemplateIn As System.Short Dim Scale1 As System.Double Dim Scale2 As System.Double Dim SkPointsFlag As System.Integer   instance.SetupSheet2(Name, PaperSize, TemplateIn, Scale1, Scale2, SkPointsFlag) ``` | |

| C# |  |
| --- | --- |
| ``` void SetupSheet2(     System.string Name,    System.short PaperSize,    System.short TemplateIn,    System.double Scale1,    System.double Scale2,    System.int SkPointsFlag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetupSheet2(  &   System.String^ Name, &   System.short PaperSize, &   System.short TemplateIn, &   System.double Scale1, &   System.double Scale2, &   System.int SkPointsFlag ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*

*PaperSize*

*TemplateIn*

*Scale1*

*Scale2*

*SkPointsFlag*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::SetupSheet2.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)