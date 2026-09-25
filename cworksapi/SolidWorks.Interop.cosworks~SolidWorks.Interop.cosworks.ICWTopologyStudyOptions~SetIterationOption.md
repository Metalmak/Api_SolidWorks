<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions~SetIterationOption.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetIterationOption Method (ICWTopologyStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions.html) : SetIterationOption Method (ICWTopologyStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIterationOption*
:   Iteration option as defined in [swsTopologyIterationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyIterationOption_e.html)

Sets the method for calculating the maximum number of iterations needed by the optimization algorithm to reach convergence.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetIterationOption( _    ByVal NIterationOption As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyStudyOptions Dim NIterationOption As System.Integer   instance.SetIterationOption(NIterationOption) ``` | |

| C# |  |
| --- | --- |
| ``` void SetIterationOption(     System.int NIterationOption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetIterationOption(  &   System.int NIterationOption ) ``` | |

#### Parameters

*NIterationOption*
:   Iteration option as defined in [swsTopologyIterationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyIterationOption_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyStudyOptions::SetIterationOption.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions.html)

[ICWTopologyStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0