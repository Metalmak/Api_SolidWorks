<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateCustomSymbol.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateCustomSymbol Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateCustomSymbol Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SegmentCount*

*Segments*

*PointCount*

*Points*

*NoteCount*

*Notes*

Obsolete. Superseded by [ISkethcManager::MakeSketchBlockFromFile](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~MakeSketchBlockFromFile.html), [ISketchManager::MakeSketchBlockSelected](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~MakeSketchBlockFromSelected.html), and [ISketchManager::MakeSketchBlockFromSketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~MakeSketchBlockFromSketch.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateCustomSymbol( _    ByVal SegmentCount As System.Integer, _    ByRef Segments As SketchSegment, _    ByVal PointCount As System.Integer, _    ByRef Points As SketchPoint, _    ByVal NoteCount As System.Integer, _    ByRef Notes As Note _ ) As CustomSymbol ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim SegmentCount As System.Integer Dim Segments As SketchSegment Dim PointCount As System.Integer Dim Points As SketchPoint Dim NoteCount As System.Integer Dim Notes As Note Dim value As CustomSymbol   value = instance.ICreateCustomSymbol(SegmentCount, Segments, PointCount, Points, NoteCount, Notes) ``` | |

| C# |  |
| --- | --- |
| ``` CustomSymbol ICreateCustomSymbol(     System.int SegmentCount,    ref SketchSegment Segments,    System.int PointCount,    ref SketchPoint Points,    System.int NoteCount,    ref Note Notes ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CustomSymbol^ ICreateCustomSymbol(  &   System.int SegmentCount, &   SketchSegment^% Segments, &   System.int PointCount, &   SketchPoint^% Points, &   System.int NoteCount, &   Note^% Notes ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SegmentCount*

*Segments*

*PointCount*

*Points*

*NoteCount*

*Notes*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateCustomSymbol.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)