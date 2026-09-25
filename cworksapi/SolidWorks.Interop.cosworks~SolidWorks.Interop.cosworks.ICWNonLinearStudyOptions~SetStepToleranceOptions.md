<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~SetStepToleranceOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetStepToleranceOptions Method (ICWNonLinearStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) : SetStepToleranceOptions Method (ICWNonLinearStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NEqilibriumIteration*
:   Frequency of performing equilibrium in number of solution steps

*NMaxEqilibriumIteration*
:   Maximum number of equilibrium iterations for any solution step

*DConvTol*
:   Relative displacement tolerance used for equilibrium convergence

*DPlasticityTol*
:   Tolerance for strain increment for models with creep or plasticity

*NSingularityEleFactor*
:   Stiffness singularity elimination factor:

    * normal solution if set to 1* if <1.0, then the program modifies stiffness terms causing singularity to help convergence

    If normal solution fails, trying a different value; for example, 0 may help convergence.

Sets convergence and equilibrium parameters.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetStepToleranceOptions( _    ByVal NEqilibriumIteration As System.Integer, _    ByVal NMaxEqilibriumIteration As System.Integer, _    ByVal DConvTol As System.Double, _    ByVal DPlasticityTol As System.Double, _    ByVal NSingularityEleFactor As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWNonLinearStudyOptions Dim NEqilibriumIteration As System.Integer Dim NMaxEqilibriumIteration As System.Integer Dim DConvTol As System.Double Dim DPlasticityTol As System.Double Dim NSingularityEleFactor As System.Double Dim value As System.Integer   value = instance.SetStepToleranceOptions(NEqilibriumIteration, NMaxEqilibriumIteration, DConvTol, DPlasticityTol, NSingularityEleFactor) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetStepToleranceOptions(     System.int NEqilibriumIteration,    System.int NMaxEqilibriumIteration,    System.double DConvTol,    System.double DPlasticityTol,    System.double NSingularityEleFactor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetStepToleranceOptions(  &   System.int NEqilibriumIteration, &   System.int NMaxEqilibriumIteration, &   System.double DConvTol, &   System.double DPlasticityTol, &   System.double NSingularityEleFactor ) ``` | |

#### Parameters

*NEqilibriumIteration*
:   Frequency of performing equilibrium in number of solution steps

*NMaxEqilibriumIteration*
:   Maximum number of equilibrium iterations for any solution step

*DConvTol*
:   Relative displacement tolerance used for equilibrium convergence

*DPlasticityTol*
:   Tolerance for strain increment for models with creep or plasticity

*NSingularityEleFactor*
:   Stiffness singularity elimination factor:

    * normal solution if set to 1* if <1.0, then the program modifies stiffness terms causing singularity to help convergence

    If normal solution fails, trying a different value; for example, 0 may help convergence.

#### Return Value

Status as defined in [swsNonLinearStudyOptionsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNonLinearStudyOptionsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWNonLinearStudyOptions::SetStepToleranceOptions.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html)

[ICWNonLinearStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions_members.html)

[ICWNonLinearStudyOptions::GetStepToleranceOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~GetStepToleranceOptions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation 2010 SP3.0