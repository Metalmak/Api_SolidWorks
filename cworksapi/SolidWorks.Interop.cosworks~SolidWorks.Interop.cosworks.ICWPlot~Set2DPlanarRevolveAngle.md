<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~Set2DPlanarRevolveAngle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| Set2DPlanarRevolveAngle Method (ICWPlot) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : Set2DPlanarRevolveAngle Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*D2DPlanarRevolveAngle*
:   Angle of revolution about a selected axis to create the 3D plot

Sets the revolve angle of the 3D plot of a 2D Simplification study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Set2DPlanarRevolveAngle( _    ByVal D2DPlanarRevolveAngle As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim D2DPlanarRevolveAngle As System.Double Dim value As System.Integer   value = instance.Set2DPlanarRevolveAngle(D2DPlanarRevolveAngle) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Set2DPlanarRevolveAngle(     System.double D2DPlanarRevolveAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Set2DPlanarRevolveAngle(  &   System.double D2DPlanarRevolveAngle ) ``` | |

#### Parameters

*D2DPlanarRevolveAngle*
:   Angle of revolution about a selected axis to create the 3D plot

#### Return Value

Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::Set2DPlanarRevolveAngle.

# ![](dotnetimages/collapse.gif)Example

See the [ICWPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only:

* for 2D Simplification axi-symmetric studies where the geometry, loads, and restraints are symmetric (360 degrees) about an axis.* if [ICWPlot::ShowAs3DPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~ShowAs3DPlot.html) is set to true.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0