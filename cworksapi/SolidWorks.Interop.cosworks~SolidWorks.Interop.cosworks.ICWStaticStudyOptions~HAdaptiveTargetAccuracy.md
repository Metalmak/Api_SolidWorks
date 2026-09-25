<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveTargetAccuracy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| HAdaptiveTargetAccuracy Property (ICWStaticStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStaticStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html) : HAdaptiveTargetAccuracy Property (ICWStaticStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the target accuracy of the h-adaptive mesh iteration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property HAdaptiveTargetAccuracy As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStaticStudyOptions Dim value As System.Double   instance.HAdaptiveTargetAccuracy = value   value = instance.HAdaptiveTargetAccuracy ``` | |

| C# |  |
| --- | --- |
| ``` System.double HAdaptiveTargetAccuracy {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double HAdaptiveTargetAccuracy {    System.double get();    void set ( &   System.double value); } ``` | |

#### Property Value

0.80 <= Target accuracy <= 0.99

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStaticStudyOptions::HAdaptiveTargetAccuracy.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ICWStaticStudyOptions::AdaptiveMethodType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~AdaptiveMethodType.html) is set to 1.

Target accuracy is the percent change in strain energy between two consecutive mesh iterations. Mesh iteration ends when two values differ by less than the target accuracy.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStaticStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html)

[ICWStaticStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions_members.html)

[ICWStaticStudyOptions::HAdaptiveAccuracyBias Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveAccuracyBias.html)

[ICWStaticStudyOptions::HAdaptiveMaxNoIterations Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveMaxNoIterations.html)

[ICWStaticStudyOptions::HAdaptiveMeshCoarsening Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveMeshCoarsening.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0