<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~ApplyNameViewOrientation2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ApplyNameViewOrientation2 Method (ICWPlot) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : ApplyNameViewOrientation2 Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NNameViewOrientation*
:   View orientation as defined in [swsNameViewOrientation\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsNameViewOrientation_e.html)

Associates this plot with the specified view orientation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ApplyNameViewOrientation2( _    ByVal NNameViewOrientation As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim NNameViewOrientation As System.Integer Dim value As System.Integer   value = instance.ApplyNameViewOrientation2(NNameViewOrientation) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ApplyNameViewOrientation2(     System.int NNameViewOrientation ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ApplyNameViewOrientation2(  &   System.int NNameViewOrientation ) ``` | |

#### Parameters

*NNameViewOrientation*
:   View orientation as defined in [swsNameViewOrientation\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsNameViewOrientation_e.html)

#### Return Value

Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::ApplyNameViewOrientation2.

# ![](dotnetimages/collapse.gif)Example

See the [ICWPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid for the following plots:

* Acceleration* Beam diagram* Displacement* Mode shape/amplitude* Fatigue* Strain* Strain energy density* Stress* Thermal* Vector

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0