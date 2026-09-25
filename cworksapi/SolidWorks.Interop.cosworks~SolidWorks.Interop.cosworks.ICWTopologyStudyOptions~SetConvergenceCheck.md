<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions~SetConvergenceCheck.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetConvergenceCheck Method (ICWTopologyStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions.html) : SetConvergenceCheck Method (ICWTopologyStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NConvergenceCheck*
:   Activation option for the convergence check as defined in [swsTopologyActivationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyActivationOption_e.html)

Sets whether to have the solver check for convergence with each iteration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetConvergenceCheck( _    ByVal NConvergenceCheck As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyStudyOptions Dim NConvergenceCheck As System.Integer   instance.SetConvergenceCheck(NConvergenceCheck) ``` | |

| C# |  |
| --- | --- |
| ``` void SetConvergenceCheck(     System.int NConvergenceCheck ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetConvergenceCheck(  &   System.int NConvergenceCheck ) ``` | |

#### Parameters

*NConvergenceCheck*
:   Activation option for the convergence check as defined in [swsTopologyActivationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyActivationOption_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyStudyOptions::SetConvergenceCheck.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions.html) example.

# ![](dotnetimages/collapse.gif)Remarks

If NConvergenceCheck is set to swsTopologyActivationOption\_e:

* ActivationOption\_Activate, then the solver checks with each iteration whether the objective or the constraint has converged. If so, then it stops the solution. Numerical tolerances between iterations are relaxed (draft quality).* ActivationOption\_Deactivate, then the solver uses a smaller numerical tolerance (high quality), and both the objective and constraint need to be satisfied for the solver to stop.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions.html)

[ICWTopologyStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0