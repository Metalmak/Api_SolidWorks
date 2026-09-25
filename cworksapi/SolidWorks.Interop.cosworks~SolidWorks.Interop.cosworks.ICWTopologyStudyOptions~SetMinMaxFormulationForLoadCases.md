<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions~SetMinMaxFormulationForLoadCases.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMinMaxFormulationForLoadCases Method (ICWTopologyStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions.html) : SetMinMaxFormulationForLoadCases Method (ICWTopologyStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NMinMaxFormulationForLoadCases*
:   Activation option for min max formulation for load cases as defined in [swsTopologyActivationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyActivationOption_e.html)

Sets whether to use the min max formulation for multiple load cases.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMinMaxFormulationForLoadCases( _    ByVal NMinMaxFormulationForLoadCases As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyStudyOptions Dim NMinMaxFormulationForLoadCases As System.Integer   instance.SetMinMaxFormulationForLoadCases(NMinMaxFormulationForLoadCases) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMinMaxFormulationForLoadCases(     System.int NMinMaxFormulationForLoadCases ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMinMaxFormulationForLoadCases(  &   System.int NMinMaxFormulationForLoadCases ) ``` | |

#### Parameters

*NMinMaxFormulationForLoadCases*
:   Activation option for min max formulation for load cases as defined in [swsTopologyActivationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyActivationOption_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyStudyOptions::SetMinMaxFormulationForLoadCases.

# ![](dotnetimages/collapse.gif)Remarks

If NMinMaxFormulationForLoadCases is set to swsTopologyActivationOption\_e.ActivationOption\_Activate, then multiple load cases (defined with the Load Case Manager) can act on a component independently.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions.html)

[ICWTopologyStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0