<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~DrawingViewRotate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DrawingViewRotate Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : DrawingViewRotate Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NewAngle*
:   New angle value for the drawing view

Rotates the selected drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DrawingViewRotate( _    ByVal NewAngle As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim NewAngle As System.Double Dim value As System.Boolean   value = instance.DrawingViewRotate(NewAngle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DrawingViewRotate(     System.double NewAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DrawingViewRotate(  &   System.double NewAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NewAngle*
:   New angle value for the drawing view

#### Return Value

True if successfully rotated, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::DrawingViewRotate.

# ![](dotnetimages/collapse.gif)Example

[Rotate Drawing View 45 Degrees (C#)](Rotate_Drawing_View_45_Degrees_Example_CSharp.htm)

[Rotate Drawing Veiw 45 Degrees (VB.NET)](Rotate_Drawing_View_45_Degrees_Example_VBNET.htm)

[Rotate Drawing View 45 Degrees (VBA)](Rotate_Drawing_View_45_Degrees_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::AlignHorz Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AlignHorz.html)

[IDrawingDoc::AlignVert Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AlignVert.html)

[IDrawingDoc::RestoreRotation Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~RestoreRotation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207