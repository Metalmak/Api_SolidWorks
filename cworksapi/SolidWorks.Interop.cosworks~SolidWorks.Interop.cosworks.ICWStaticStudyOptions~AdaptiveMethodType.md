<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~AdaptiveMethodType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AdaptiveMethodType Property (ICWStaticStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStaticStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html) : AdaptiveMethodType Property (ICWStaticStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the type of adaptive meshing to use to achieve more accurate results.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AdaptiveMethodType As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStaticStudyOptions Dim value As System.Integer   instance.AdaptiveMethodType = value   value = instance.AdaptiveMethodType ``` | |

| C# |  |
| --- | --- |
| ``` System.int AdaptiveMethodType {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int AdaptiveMethodType {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

* 0 = None* 1 = h-adaptive; iteratively adjusts the size of the mesh cell in areas of the model where a smaller mesh is needed* 2 = p-adaptive; iteratively adjusts the polynomial order of the mesh to improve accuracy

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStaticStudyOptions::AdaptiveMethodType.

# ![](dotnetimages/collapse.gif)Example

See the [ICWStaticStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

If you set this property to 2, you must set [ICWMesh::Quality](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~Quality.html) to [swsMeshQuality\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshQuality_e.html).swsMeshQualityHigh.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStaticStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html)

[ICWStaticStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions_members.html)

[ICWStaticStudyOptions::HAdaptiveAccuracyBias Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveAccuracyBias.html)

[ICWStaticStudyOptions::HAdaptiveMaxNoIterations Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveMaxNoIterations.html)

[ICWStaticStudyOptions::HAdaptiveMeshCoarsening Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveMeshCoarsening.html)

[ICWStaticStudyOptions::HAdaptiveTargetAccuracy Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveTargetAccuracy.html)

[ICWStaticStudyOptions::PAdaptiveConvergenceCriteria Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveConvergenceCriteria.html)

[ICWStaticStudyOptions::PAdaptiveErrorLimit Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveErrorLimit.html)

[ICWStaticStudyOptions::PAdaptiveMaxIterations Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveMaxIterations.html)

[ICWStaticStudyOptions::PAdaptiveMaxPOrder Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveMaxPOrder.html)

[ICWStaticStudyOptions::PAdaptiveStartingPOrder Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveStartingPOrder.html)

[ICWStaticStudyOptions::PAdaptiveStrainEnergyErrorLimit Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveStrainEnergyErrorLimit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0