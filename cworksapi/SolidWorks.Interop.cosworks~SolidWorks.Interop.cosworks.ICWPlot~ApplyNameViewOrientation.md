<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~ApplyNameViewOrientation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ApplyNameViewOrientation Method (ICWPlot) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : ApplyNameViewOrientation Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SNameViewOrientation*
:   Name view orientation

Obsolete. Superseded by [ICWPlot::ApplyNameViewOrientation2.](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~ApplyNameViewOrientation2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ApplyNameViewOrientation( _    ByVal SNameViewOrientation As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim SNameViewOrientation As System.String Dim value As System.Integer   value = instance.ApplyNameViewOrientation(SNameViewOrientation) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ApplyNameViewOrientation(     System.string SNameViewOrientation ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ApplyNameViewOrientation(  &   System.String^ SNameViewOrientation ) ``` | |

#### Parameters

*SNameViewOrientation*
:   Name view orientation

#### Return Value

Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::ApplyNameViewOrientation.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid for the following plots:

* Acceleration* Beam diagram* Displacement* Mode shape/amplitude* Fatigue* Strain* Strain energy density* Stress* Thermal* Vector

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0