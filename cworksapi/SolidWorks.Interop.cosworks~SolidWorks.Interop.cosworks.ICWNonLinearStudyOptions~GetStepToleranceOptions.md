<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~GetStepToleranceOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetStepToleranceOptions Method (ICWNonLinearStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) : GetStepToleranceOptions Method (ICWNonLinearStudyOptions) |

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

Gets convergence and equilibrium parameters.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetStepToleranceOptions( _    ByRef NEqilibriumIteration As System.Integer, _    ByRef NMaxEqilibriumIteration As System.Integer, _    ByRef DConvTol As System.Double, _    ByRef DPlasticityTol As System.Double, _    ByRef NSingularityEleFactor As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWNonLinearStudyOptions Dim NEqilibriumIteration As System.Integer Dim NMaxEqilibriumIteration As System.Integer Dim DConvTol As System.Double Dim DPlasticityTol As System.Double Dim NSingularityEleFactor As System.Double   instance.GetStepToleranceOptions(NEqilibriumIteration, NMaxEqilibriumIteration, DConvTol, DPlasticityTol, NSingularityEleFactor) ``` | |

| C# |  |
| --- | --- |
| ``` void GetStepToleranceOptions(     out System.int NEqilibriumIteration,    out System.int NMaxEqilibriumIteration,    out System.double DConvTol,    out System.double DPlasticityTol,    out System.double NSingularityEleFactor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetStepToleranceOptions(  &   [Out] System.int NEqilibriumIteration, &   [Out] System.int NMaxEqilibriumIteration, &   [Out] System.double DConvTol, &   [Out] System.double DPlasticityTol, &   [Out] System.double NSingularityEleFactor ) ``` | |

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

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWNonLinearStudyOptions::GetStepToleranceOptions.

# ![](dotnetimages/collapse.gif)Example

See the [ICWNonLinearStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html)

[ICWNonLinearStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions_members.html)

[ICWNonLinearStudyOptions::SetStepToleranceOptions Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~SetStepToleranceOptions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation 2010 SP3.0