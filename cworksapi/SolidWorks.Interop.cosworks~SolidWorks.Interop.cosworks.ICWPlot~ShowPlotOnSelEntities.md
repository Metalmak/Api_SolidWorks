<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~ShowPlotOnSelEntities.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ShowPlotOnSelEntities Method (ICWPlot) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : ShowPlotOnSelEntities Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BSelFaceOnly*
:   True to display plot only for ArraySelectedEntities, false to display plot for all entities

*ArraySelectedEntities*
:   Array of selected faces and bodies; valid only if BSelFaceOnly is true

Sets whether to display this plot only for selected entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ShowPlotOnSelEntities( _    ByVal BSelFaceOnly As System.Boolean, _    ByVal ArraySelectedEntities As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim BSelFaceOnly As System.Boolean Dim ArraySelectedEntities As System.Object Dim value As System.Integer   value = instance.ShowPlotOnSelEntities(BSelFaceOnly, ArraySelectedEntities) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ShowPlotOnSelEntities(     System.bool BSelFaceOnly,    System.object ArraySelectedEntities ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ShowPlotOnSelEntities(  &   System.bool BSelFaceOnly, &   System.Object^ ArraySelectedEntities ) ``` | |

#### Parameters

*BSelFaceOnly*
:   True to display plot only for ArraySelectedEntities, false to display plot for all entities

*ArraySelectedEntities*
:   Array of selected faces and bodies; valid only if BSelFaceOnly is true

#### Return Value

Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::ShowPlotOnSelEntities.

# ![](dotnetimages/collapse.gif)Example

See the [ICWPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid for the following plots only if [ICWPlot::ShowShellin3D](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~ShowShellin3D.html)  and [ICWPlot::ShowTensorOrVector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~ShowTensorOrVector.html) are both false:

* Acceleration* Displacement* Mode shape/amplitude* Strain* Stress* Velocity

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0