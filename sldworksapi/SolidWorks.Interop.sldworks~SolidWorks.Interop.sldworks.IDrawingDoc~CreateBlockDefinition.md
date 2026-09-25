<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateBlockDefinition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateBlockDefinition Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateBlockDefinition Method (IDrawingDoc) |

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

*Segments*

*Points*

*Notes*

*Dimensions*

*Blocks*

Obsolete. Superseded by [ISketchManager::MakeSketchBlockFromFile](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~MakeSketchBlockFromFile.html), [ISketchManager::MakeSketchBlockSelected](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~MakeSketchBlockFromSelected.html), and [ISketchManager::MakeSketchBlockFromSketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~MakeSketchBlockFromSketch.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateBlockDefinition( _    ByVal Name As System.String, _    ByVal XRefFileName As System.String, _    ByVal Instance As System.Boolean, _    ByVal Segments As System.Object, _    ByVal Points As System.Object, _    ByVal Notes As System.Object, _    ByVal Dimensions As System.Object, _    ByVal Blocks As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Name As System.String Dim XRefFileName As System.String Dim Instance As System.Boolean Dim Segments As System.Object Dim Points As System.Object Dim Notes As System.Object Dim Dimensions As System.Object Dim Blocks As System.Object Dim value As System.Object   value = instance.CreateBlockDefinition(Name, XRefFileName, Instance, Segments, Points, Notes, Dimensions, Blocks) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateBlockDefinition(     System.string Name,    System.string XRefFileName,    System.bool Instance,    System.object Segments,    System.object Points,    System.object Notes,    System.object Dimensions,    System.object Blocks ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateBlockDefinition(  &   System.String^ Name, &   System.String^ XRefFileName, &   System.bool Instance, &   System.Object^ Segments, &   System.Object^ Points, &   System.Object^ Notes, &   System.Object^ Dimensions, &   System.Object^ Blocks ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*

*XRefFileName*

*Instance*

*Segments*

*Points*

*Notes*

*Dimensions*

*Blocks*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateBlockDefinition.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)