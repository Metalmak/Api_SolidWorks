<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SaveDisplacementsAndVelocitiesOption.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SaveDisplacementsAndVelocitiesOption Property (ICWStudyResultOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) : SaveDisplacementsAndVelocitiesOption Property (ICWStudyResultOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the displacement and velocity option.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property SaveDisplacementsAndVelocitiesOption As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyResultOptions Dim value As System.Integer   instance.SaveDisplacementsAndVelocitiesOption = value   value = instance.SaveDisplacementsAndVelocitiesOption ``` | |

| C# |  |
| --- | --- |
| ``` System.int SaveDisplacementsAndVelocitiesOption {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int SaveDisplacementsAndVelocitiesOption {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Option as defined in [swsResultsDisplacementAndVelocityOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsDisplacementAndVelocityOption_e.html) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyResultOptions::SaveDisplacementsAndVelocitiesOption.

# ![](dotnetimages/collapse.gif)Example

See the [ICWStudyResultOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only for linear dynamic studies and only if [ICWStudyResultOptions::SaveResultsForSolutionStepsOption](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStudyResultOptions~SaveResultsForSolutionStepsOption.html) = swsSaveResultsOption\_e.swsSaveResultsOption\_ForSpecifiedSolutionSteps.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html)

[ICWStudyResultOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions_members.html)

[ICWStudyResultOptions::SaveReactions Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SaveReactions.html)

[ICWStudyResultOptions::SaveStresses Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SaveStresses.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0