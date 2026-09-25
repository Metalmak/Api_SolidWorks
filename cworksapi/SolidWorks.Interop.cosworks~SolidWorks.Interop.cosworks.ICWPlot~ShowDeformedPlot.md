<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~ShowDeformedPlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ShowDeformedPlot Method (ICWPlot) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : ShowDeformedPlot Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BShowDeformed*
:   True to plot on the deformed shape, false to not

*NDeformOption*
:   Deformed shape option as defined in [swsDeformType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDeformType_e.html)

*DUserDefValue*
:   User-defined scale factor; valid only if NDeformOption is swsDeformType\_e.swsUserDefined

*BShowColors*
:   True to show colors, false to not

Sets whether and how to plot on the deformed shape of the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ShowDeformedPlot( _    ByVal BShowDeformed As System.Boolean, _    ByVal NDeformOption As System.Integer, _    ByVal DUserDefValue As System.Double, _    ByVal BShowColors As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim BShowDeformed As System.Boolean Dim NDeformOption As System.Integer Dim DUserDefValue As System.Double Dim BShowColors As System.Boolean Dim value As System.Integer   value = instance.ShowDeformedPlot(BShowDeformed, NDeformOption, DUserDefValue, BShowColors) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ShowDeformedPlot(     System.bool BShowDeformed,    System.int NDeformOption,    System.double DUserDefValue,    System.bool BShowColors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ShowDeformedPlot(  &   System.bool BShowDeformed, &   System.int NDeformOption, &   System.double DUserDefValue, &   System.bool BShowColors ) ``` | |

#### Parameters

*BShowDeformed*
:   True to plot on the deformed shape, false to not

*NDeformOption*
:   Deformed shape option as defined in [swsDeformType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDeformType_e.html)

*DUserDefValue*
:   User-defined scale factor; valid only if NDeformOption is swsDeformType\_e.swsUserDefined

*BShowColors*
:   True to show colors, false to not

#### Return Value

Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::ShowDeformedPlot.

# ![](dotnetimages/collapse.gif)Example

See the [ICWPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid for the following plots:

* Acceleration* Displacement* Mode shape/amplitude* Strain* Strain energy density* Stress* Vector

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0