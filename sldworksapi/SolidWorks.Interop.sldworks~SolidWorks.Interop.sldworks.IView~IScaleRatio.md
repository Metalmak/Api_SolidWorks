<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IScaleRatio.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IScaleRatio Property (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : IScaleRatio Property (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the scale of the drawing view, returning the results in ratio format (n:n).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property IScaleRatio As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim value As System.Double   instance.IScaleRatio = value   value = instance.IScaleRatio ``` | |

| C# |  |
| --- | --- |
| ``` System.double IScaleRatio {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double IScaleRatio {    System.double get();    void set ( &   System.double value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array of 2 doubles (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::IScaleRatio.

# ![](dotnetimages/collapse.gif)Remarks

The two values represent the two numbers if the scale is described as a ratio. The first value is the numerator; the second value is the denominator. This is what the scale is when represented as n:n.

This property and [IView::ScaleDecimal](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~ScaleDecimal.html) contain the same information, but use the value in a different form.

* IView::ScaleRatio returns the scale as a ratio of two numbers.

  * IView::ScaleDecimal returns the scale as a decimal number.

For example, if View::ScaleRatio returns 3 2 or 3:2, then IView::ScaleDecimal would return 1.5.

Changing this property may cause changes to the graphics of the drawing. After making all of the view-related changes, call [IModelDoc2::EditRebuild3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~EditRebuild3.html) to regenerate the drawing to see these changes.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::UseParentScale Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~UseParentScale.html)

[IView::UseSheetScale Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~UseSheetScale.html)

[IView::ScaleRatio Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~ScaleRatio.html)