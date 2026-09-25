<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~SetXform.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetXform Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : SetXform Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Transform*
:   Array of 3 doubles (see **Remarks**)

Sets the matrix used for display of this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetXform( _    ByVal Transform As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim Transform As System.Object Dim value As System.Boolean   value = instance.SetXform(Transform) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetXform(     System.object Transform ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetXform(  &   System.Object^ Transform ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Transform*
:   Array of 3 doubles (see **Remarks**)

#### Return Value

True if transform successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::SetXform.

# ![](dotnetimages/collapse.gif)Remarks

The 3 doubles are the X and Y position of the view, relative to the sheet origin, and the scale of the view.

Any view alignments that might affect this view are handled the same way as if you were using the user interface to draw the view to move it. If it is aligned with another view, then it will only move along the alignment vector. If it has child views that are aligned with it, then those views will also be moved along with this view.

Calling this method is equivalent to setting the [IView::Position](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~Position.html) or [IView::IPosition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IPosition.html) property (to set X and Y), and the [IView::ScaleDecimal](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~ScaleDecimal.html) property (to set the scale).

To get the view matrix, use [IView::GetXform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetXform.html) or [IView::IGetXform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetXform.html) method.

Using this method may cause changes to the graphics of the drawing. Once all the view-related changes have been made, the user should call [IModelDoc2::EditRebuild3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~EditRebuild3.html) to regenerate the drawing, in order to see these changes.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::ISetXform Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~ISetXform.html)

[IView::GetXform Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetXform.html)

[IView::IGetXform Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetXform.html)