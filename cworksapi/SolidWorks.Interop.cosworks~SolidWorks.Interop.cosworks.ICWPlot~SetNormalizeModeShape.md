<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~SetNormalizeModeShape.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetNormalizeModeShape Method (ICWPlot) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : SetNormalizeModeShape Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BNormModeShape*
:   True to normalize the mode shape (maximum amplitude is 1), false to not

Sets whether to normalize the mode shape of this plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetNormalizeModeShape( _    ByVal BNormModeShape As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim BNormModeShape As System.Boolean Dim value As System.Integer   value = instance.SetNormalizeModeShape(BNormModeShape) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetNormalizeModeShape(     System.bool BNormModeShape ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetNormalizeModeShape(  &   System.bool BNormModeShape ) ``` | |

#### Parameters

*BNormModeShape*
:   True to normalize the mode shape (maximum amplitude is 1), false to not

#### Return Value

Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::SetNormalizeModeShape.

# ![](dotnetimages/collapse.gif)Example

See the [ICWPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for amplitude plots.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

[ICWPlot::SetModeShape Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~SetModeShape.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0