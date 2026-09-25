<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~DragModelDimension.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DragModelDimension Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : DragModelDimension Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ViewName*
:   Name of the drawing view to which you want to copy or move the selected model dimension

*DropEffect*
:   * Copy = 1* Move = 2

*X*
:   X location in sheet space for the newly copied or moved dimension

*Y*
:   Y location in sheet space for the newly copied or moved dimension

*Z*
:   Z location in sheet space for the newly copied or moved dimension; set to  0

Copies or moves dimensions to a different drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub DragModelDimension( _    ByVal ViewName As System.String, _    ByVal DropEffect As System.Short, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim ViewName As System.String Dim DropEffect As System.Short Dim X As System.Double Dim Y As System.Double Dim Z As System.Double   instance.DragModelDimension(ViewName, DropEffect, X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` void DragModelDimension(     System.string ViewName,    System.short DropEffect,    System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DragModelDimension(  &   System.String^ ViewName, &   System.short DropEffect, &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ViewName*
:   Name of the drawing view to which you want to copy or move the selected model dimension

*DropEffect*
:   * Copy = 1* Move = 2

*X*
:   X location in sheet space for the newly copied or moved dimension

*Y*
:   Y location in sheet space for the newly copied or moved dimension

*Z*
:   Z location in sheet space for the newly copied or moved dimension; set to  0

#### Return Value

The ViewName argument cannot be the current view for the dimension.

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::DragModelDimension.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::Dimensions Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~Dimensions.html)