<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~UseParentScale.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UseParentScale Property (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : UseParentScale Property (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the drawing view's scale to match the parent drawing view's scale.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property UseParentScale As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim value As System.Boolean   instance.UseParentScale = value   value = instance.UseParentScale ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UseParentScale {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool UseParentScale {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True if the drawing view's scale is set to be the same as the parent's drawing view scale, false if the drawing view scale is independent of the parent's drawing view scale

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::UseParentScale.

# ![](dotnetimages/collapse.gif)Example

[Set View Scale Opposite Parent View Scale (VBA)](Set_View_Scale_Opposite_Parent_View_Scale_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Changing this property can cause changes to the graphics of the drawing. After making all of the view-related changes, call the [IModelDoc2::EditRebuild3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~EditRebuild3.html) method to regenerate the drawing to see these changes.

To set the drawing view's scale to be the same as the drawing sheet's scale, use [IView::UseSheetScale](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~UseSheetScale.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::IScaleRatio Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IScaleRatio.html)

[IView::ScaleRatio Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~ScaleRatio.html)

[IView::ScaleDecimal Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~ScaleDecimal.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP5, Revision Number 12.5