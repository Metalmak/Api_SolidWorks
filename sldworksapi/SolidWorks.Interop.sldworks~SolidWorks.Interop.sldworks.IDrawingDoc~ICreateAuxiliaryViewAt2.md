<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateAuxiliaryViewAt2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateAuxiliaryViewAt2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateAuxiliaryViewAt2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   X position for the auxiliary view

*Y*
:   Y position for the auxiliary view

*Z*
:   Z position for the auxiliary view

*NotAligned*
:   True aligns the view from its owner, false does not

*Label*
:   String that holds label of the auxiliary view

*Showarrow*
:   True shows the arrow, false hides the arrow

*Flip*
:   True flips the side shown in the auxiliary view, false does not

Creates an auxiliary view based on a selected edge in a drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateAuxiliaryViewAt2( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByVal NotAligned As System.Boolean, _    ByVal Label As System.String, _    ByVal Showarrow As System.Boolean, _    ByVal Flip As System.Boolean _ ) As View ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim NotAligned As System.Boolean Dim Label As System.String Dim Showarrow As System.Boolean Dim Flip As System.Boolean Dim value As View   value = instance.ICreateAuxiliaryViewAt2(X, Y, Z, NotAligned, Label, Showarrow, Flip) ``` | |

| C# |  |
| --- | --- |
| ``` View ICreateAuxiliaryViewAt2(     System.double X,    System.double Y,    System.double Z,    System.bool NotAligned,    System.string Label,    System.bool Showarrow,    System.bool Flip ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` View^ ICreateAuxiliaryViewAt2(  &   System.double X, &   System.double Y, &   System.double Z, &   System.bool NotAligned, &   System.String^ Label, &   System.bool Showarrow, &   System.bool Flip ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   X position for the auxiliary view

*Y*
:   Y position for the auxiliary view

*Z*
:   Z position for the auxiliary view

*NotAligned*
:   True aligns the view from its owner, false does not

*Label*
:   String that holds label of the auxiliary view

*Showarrow*
:   True shows the arrow, false hides the arrow

*Flip*
:   True flips the side shown in the auxiliary view, false does not

#### Return Value

Pointer to the newly created auxiliary [view](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateAuxiliaryViewAt2.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::CreateAuxiliaryViewAt2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateAuxiliaryViewAt2.html)

[IDrawingDoc::CreateDetailViewAt3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateDetailViewAt3.html)

[IDrawingDoc::ICreateDetailViewAt3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateDetailViewAt3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0