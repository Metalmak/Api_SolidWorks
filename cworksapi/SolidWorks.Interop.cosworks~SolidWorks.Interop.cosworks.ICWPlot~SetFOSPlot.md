<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~SetFOSPlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFOSPlot Method (ICWPlot) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : SetFOSPlot Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BFOSPlot*
:   True to plot the factor of safety throughout the model, false to not

Sets whether to plot the factor of safety throughout the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFOSPlot( _    ByVal BFOSPlot As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim BFOSPlot As System.Boolean Dim value As System.Integer   value = instance.SetFOSPlot(BFOSPlot) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetFOSPlot(     System.bool BFOSPlot ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetFOSPlot(  &   System.bool BFOSPlot ) ``` | |

#### Parameters

*BFOSPlot*
:   True to plot the factor of safety throughout the model, false to not

#### Return Value

Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::SetFOSPlot.

# ![](dotnetimages/collapse.gif)Example

See the [ICWPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0