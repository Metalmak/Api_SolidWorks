<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~AlignWithView.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AlignWithView Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : AlignWithView Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AlignType*
:   Type of alignment to set as defined by swAlignViewTypes\_e

*BaseView*
:   [View](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html) with which to align, if aligning with another view

Sets view alignment.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AlignWithView( _    ByVal AlignType As System.Integer, _    ByVal BaseView As View _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim AlignType As System.Integer Dim BaseView As View Dim value As System.Boolean   value = instance.AlignWithView(AlignType, BaseView) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AlignWithView(     System.int AlignType,    View BaseView ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AlignWithView(  &   System.int AlignType, &   View^ BaseView ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AlignType*
:   Type of alignment to set as defined by swAlignViewTypes\_e

*BaseView*
:   [View](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html) with which to align, if aligning with another view

#### Return Value

True if view alignment is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::AlignWithView.

# ![](dotnetimages/collapse.gif)Example

[Align Drawing Views (C#)](Align_Drawing_Views_Example_CSharp.htm)

[Align Drawing Views (VB.NET)](Align_Drawing_Views_Example_VBNET.htm)

[Align Drawing Views (VBA)](Align_Drawing_Views_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

AlignType tells how to align this view.

|  |  |
| --- | --- |
| **If AlignType is set to...** | **Then BaseView...** |
| swAlignViewHorizontalCenter | must be specified as the view with which to align. |
| swAlignViewVerticalCenter | must be specified as the view with which to align. |
| swAlignViewHorizontalOrigin | must be specified as the view with which to align. |
| swAlignViewVerticalOrigin | must be specified as the view with which to align. |
| swNoViewAlignment | is ignored. |
| swDefaultViewAlignment | is ignored. |

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetAlignment Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetAlignment.html)

[IView::RemoveAlignment Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~RemoveAlignment.html)

[IView::UseDefaultAlignment Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~UseDefaultAlignment.html)

[IView::AlignDrawingView Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~AlignDrawingView.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0