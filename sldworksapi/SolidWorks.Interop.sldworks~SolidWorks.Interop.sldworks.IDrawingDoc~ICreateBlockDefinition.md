<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateBlockDefinition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateBlockDefinition Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateBlockDefinition Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*

*XRefFileName*

*Instance*

*SegmentCount*

*Segments*

*PointCount*

*Points*

*NoteCount*

*Notes*

*DimensionCount*

*Dimensions*

*BlockCount*

*Blocks*

Obsolete. Superseded by [ISketchManager::MakeSketchBlockFromFile](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~MakeSketchBlockFromFile.html), [ISketchManager::MakeSketchBlockSelected](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~MakeSketchBlockFromSelected.html), and [ISketchManager::MakeSketchBlockFromSketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~MakeSketchBlockFromSketch.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateBlockDefinition( _    ByVal Name As System.String, _    ByVal XRefFileName As System.String, _    ByVal Instance As System.Boolean, _    ByVal SegmentCount As System.Integer, _    ByRef Segments As SketchSegment, _    ByVal PointCount As System.Integer, _    ByRef Points As SketchPoint, _    ByVal NoteCount As System.Integer, _    ByRef Notes As Note, _    ByVal DimensionCount As System.Integer, _    ByRef Dimensions As DisplayDimension, _    ByVal BlockCount As System.Integer, _    ByRef Blocks As BlockInstance _ ) As BlockDefinition ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Name As System.String Dim XRefFileName As System.String Dim Instance As System.Boolean Dim SegmentCount As System.Integer Dim Segments As SketchSegment Dim PointCount As System.Integer Dim Points As SketchPoint Dim NoteCount As System.Integer Dim Notes As Note Dim DimensionCount As System.Integer Dim Dimensions As DisplayDimension Dim BlockCount As System.Integer Dim Blocks As BlockInstance Dim value As BlockDefinition   value = instance.ICreateBlockDefinition(Name, XRefFileName, Instance, SegmentCount, Segments, PointCount, Points, NoteCount, Notes, DimensionCount, Dimensions, BlockCount, Blocks) ``` | |

| C# |  |
| --- | --- |
| ``` BlockDefinition ICreateBlockDefinition(     System.string Name,    System.string XRefFileName,    System.bool Instance,    System.int SegmentCount,    ref SketchSegment Segments,    System.int PointCount,    ref SketchPoint Points,    System.int NoteCount,    ref Note Notes,    System.int DimensionCount,    ref DisplayDimension Dimensions,    System.int BlockCount,    ref BlockInstance Blocks ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` BlockDefinition^ ICreateBlockDefinition(  &   System.String^ Name, &   System.String^ XRefFileName, &   System.bool Instance, &   System.int SegmentCount, &   SketchSegment^% Segments, &   System.int PointCount, &   SketchPoint^% Points, &   System.int NoteCount, &   Note^% Notes, &   System.int DimensionCount, &   DisplayDimension^% Dimensions, &   System.int BlockCount, &   BlockInstance^% Blocks ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*

*XRefFileName*

*Instance*

*SegmentCount*

*Segments*

*PointCount*

*Points*

*NoteCount*

*Notes*

*DimensionCount*

*Dimensions*

*BlockCount*

*Blocks*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateBlockDefinition.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)