<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~ScaleDecimal.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ScaleDecimal Property (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : ScaleDecimal Property (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the scale of the drawing view, returning the results in decimal format.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ScaleDecimal As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim value As System.Double   instance.ScaleDecimal = value   value = instance.ScaleDecimal ``` | |

| C# |  |
| --- | --- |
| ``` System.double ScaleDecimal {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double ScaleDecimal {    System.double get();    void set ( &   System.double value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Drawing view scale

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::ScaleDecimal.

# ![](dotnetimages/collapse.gif)Example

[Set View Scale (VBA)](Set_View_Scale_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

[IView::ScaleRatio](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~ScaleRatio.html) or [IView::IScaleRatio](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IScaleRatio.html) and this property contain the same information, but use the value in different ways:

* IView::ScaleRatio gets or sets the scale as a ratio of two numbers.

  * IView::ScaleDecimal returns the scale as a decimal number.

For example, if View::ScaleRatio returns 3 2 or 3:2, then IView::ScaleDecimal would return 1.5.

Changing this property can cause changes to the graphics of the drawing. After making all the of the view-related changes, call the [IModelDoc2::EditRebuild2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~EditRebuild3.html) method to regenerate the drawing to see these changes.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::UseParentScale Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~UseParentScale.html)

[IView::UseSheetScale Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~UseSheetScale.html)