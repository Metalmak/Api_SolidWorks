<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateViewport3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateViewport3 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateViewport3 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LowerLeftX*
:   x value for lower-left coordinate for the view

*LowerLeftY*
:   y value for lower-left coordinate for the view

*SketchSize*
:   Approximate number of entries

*Scale*
:   Scale to use for the view

Creates a an empty view in a drawing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateViewport3( _    ByVal LowerLeftX As System.Double, _    ByVal LowerLeftY As System.Double, _    ByVal SketchSize As System.Short, _    ByVal Scale As System.Double _ ) As View ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim LowerLeftX As System.Double Dim LowerLeftY As System.Double Dim SketchSize As System.Short Dim Scale As System.Double Dim value As View   value = instance.CreateViewport3(LowerLeftX, LowerLeftY, SketchSize, Scale) ``` | |

| C# |  |
| --- | --- |
| ``` View CreateViewport3(     System.double LowerLeftX,    System.double LowerLeftY,    System.short SketchSize,    System.double Scale ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` View^ CreateViewport3(  &   System.double LowerLeftX, &   System.double LowerLeftY, &   System.short SketchSize, &   System.double Scale ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LowerLeftX*
:   x value for lower-left coordinate for the view

*LowerLeftY*
:   y value for lower-left coordinate for the view

*SketchSize*
:   Approximate number of entries

*Scale*
:   Scale to use for the view

#### Return Value

Pointer to the newly created [IView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateViewport3.

# ![](dotnetimages/collapse.gif)Remarks

You cannot set the size of an empty view or resize it. Instead, resizing of the view occurs automatically when you add sketch or model geometry to the view.

The center of the empty view is computed from the specified lower-left corner and default values for the upper-right corner. The latter is set to (0.001, 0.001). The center is computed as follows:

> center = lower-left\_corner + (upper-right\_corner - lower-left\_corner) / 2.0

To move the view, use [IView::Position](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~Position.html) or [IView::IPosition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IPosition.html).

The default SketchSize value is 0. If you are creating more than 500 sketch entities, specify a value instead of using the default.

After you use this method, you can create sketch entities in the new view. One advantage is that users can move the entities around the drawing by dragging the view instead of selecting all the entities.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::Create1stAngleViews2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~Create1stAngleViews2.html)

[IDrawingDoc::Create3rdAngleViews2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~Create3rdAngleViews2.html)

[IDrawingDoc::CreateAuxiliaryViewAt2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateAuxiliaryViewAt2.html)

[IDrawingDoc::CreateDetailViewAt3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateDetailViewAt3.html)

[IDrawingDoc::CreateDrawViewFromModelView3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateDrawViewFromModelView3.html)

[IDrawingDoc::CreateFlatPatternViewFromModelView2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateFlatPatternViewFromModelView2.html)

[IDrawingDoc::CreateRelativeView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateRelativeView.html)

[IDrawingDoc::CreateSectionView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateSectionView.html)

[IDrawingDoc::CreateSectionViewAt4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateSectionViewAt4.html)

[IDrawingDoc::CreateUnfoldedViewAt3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateUnfoldedViewAt3.html)

[IDrawingDoc::ICreateAuxiliaryViewAt2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateAuxiliaryViewAt2.html)

[IDrawingDoc::ICreateDetailViewAt3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateDetailViewAt3.html)

[IDrawingDoc::ICreateSectionViewAt4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateSectionViewAt4.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 SP2, Revision Number 13.2