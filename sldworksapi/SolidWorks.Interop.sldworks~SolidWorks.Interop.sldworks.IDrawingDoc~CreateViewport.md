<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateViewport.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateViewport Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateViewport Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LowerLeftX*

*LowerLeftY*

*UpperRightX*

*UpperRightY*

*SketchSize*

Obsolete. Superseded by [IDrawingDoc::CreateViewport3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateViewport3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateViewport( _    ByVal LowerLeftX As System.Double, _    ByVal LowerLeftY As System.Double, _    ByVal UpperRightX As System.Double, _    ByVal UpperRightY As System.Double, _    ByVal SketchSize As System.Short _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim LowerLeftX As System.Double Dim LowerLeftY As System.Double Dim UpperRightX As System.Double Dim UpperRightY As System.Double Dim SketchSize As System.Short Dim value As System.String   value = instance.CreateViewport(LowerLeftX, LowerLeftY, UpperRightX, UpperRightY, SketchSize) ``` | |

| C# |  |
| --- | --- |
| ``` System.string CreateViewport(     System.double LowerLeftX,    System.double LowerLeftY,    System.double UpperRightX,    System.double UpperRightY,    System.short SketchSize ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ CreateViewport(  &   System.double LowerLeftX, &   System.double LowerLeftY, &   System.double UpperRightX, &   System.double UpperRightY, &   System.short SketchSize ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LowerLeftX*

*LowerLeftY*

*UpperRightX*

*UpperRightY*

*SketchSize*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateViewport.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)