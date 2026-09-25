<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~SetPlotStepNumber.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetPlotStepNumber Method (ICWPlot) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : SetPlotStepNumber Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NStepNumber*
:   Number of solution step to plot

Sets the number of the solution step to plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPlotStepNumber( _    ByVal NStepNumber As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim NStepNumber As System.Integer Dim value As System.Integer   value = instance.SetPlotStepNumber(NStepNumber) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPlotStepNumber(     System.int NStepNumber ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPlotStepNumber(  &   System.int NStepNumber ) ``` | |

#### Parameters

*NStepNumber*
:   Number of solution step to plot

#### Return Value

Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::SetPlotStepNumber.

# ![](dotnetimages/collapse.gif)Example

[Create Nonlinear Dynamic Plots (VBA)](Create_Nonlinear_Dynamic_Plots_Example_VB.htm)

[Create Nonlinear Dynamic Plots (VB.NET)](Create_Nonlinear_Dynamic_Plots_Example_VBNET.htm)

[Create Nonlinear Dynamic Plots (C#)](Create_Nonlinear_Dynamic_Plots_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for the following plots:

* Acceleration* Displacement* Strain* Stress* Transient thermal* Velocity

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0