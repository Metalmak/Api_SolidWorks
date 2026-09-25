<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWStaticStudyOptions Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWStaticStudyOptions Interface |

The following tables list the members exposed by [ICWStaticStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AdaptiveMethodType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~AdaptiveMethodType.html) | Gets or sets the type of adaptive meshing to use to achieve more accurate results. |
| ![ Property](dotnetimages/Property.gif) | [CheckFlowPressure](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~CheckFlowPressure.html) | Obsolete. Superseded by [ICWStaticStudyOptions::CheckFlowPressure2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~CheckFlowPressure2.html). |
| ![ Property](dotnetimages/Property.gif) | [CheckFlowPressure2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~CheckFlowPressure2.html) | Gets or sets whether to import fluid pressure loads from a SOLIDWORKS Flow Simulation results file. |
| ![ Property](dotnetimages/Property.gif) | [CheckRunAsLegacy](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~CheckRunAsLegacy.html) | Obsolete. Superseded by [ICWStaticStudyOptions::CheckRunAsLegacy2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~CheckRunAsLegacy2.html). |
| ![ Property](dotnetimages/Property.gif) | [CheckRunAsLegacy2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~CheckRunAsLegacy2.html) | Gets or sets whether to run as legacy and import only the normal component of the pressure load from a SOLIDWORKS Flow Simulation results file. |
| ![ Property](dotnetimages/Property.gif) | [ComputeFreeBodyForce](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~ComputeFreeBodyForce.html) | Obsolete. Superseded by [ICWStaticStudyOptions::ComputeFreeBodyForce2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~ComputeFreeBodyForce2.html). |
| ![ Property](dotnetimages/Property.gif) | [ComputeFreeBodyForce2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~ComputeFreeBodyForce2.html) | Gets or sets whether to prepare the grid force balance at every node. |
| ![ Property](dotnetimages/Property.gif) | [DefinedReferencePressure](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~DefinedReferencePressure.html) | Gets or sets the reference pressure offset to subtract from imported pressure values. |
| ![ Property](dotnetimages/Property.gif) | [EMail](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMail.html) | Obsolete. Superseded by [ICWStaticStudyOptions::EMail2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMail2.html). |
| ![ Property](dotnetimages/Property.gif) | [EMail2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMail2.html) | Gets or sets whether to email notifications during simulations. |
| ![ Property](dotnetimages/Property.gif) | [EMailInterval](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMailInterval.html) | Gets or sets the time interval for sending email notifications during simulations. |
| ![ Property](dotnetimages/Property.gif) | [EMailIntervalUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMailIntervalUnit.html) | Gets or sets the units of time for [ICWStaticStudyOptions::EMailInterval](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMailInterval.html). |
| ![ Property](dotnetimages/Property.gif) | [EMailTimebased](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMailTimebased.html) | Obsolete. Superseded by [ICWStaticStudyOptions::EMailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMailTimebased2.html). |
| ![ Property](dotnetimages/Property.gif) | [EMailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMailTimebased2.html) | Gets or sets whether to send email notifications during simulations. |
| ![ Property](dotnetimages/Property.gif) | [EMailTo](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~EMailTo.html) | Gets or sets the recipient of email notifications. |
| ![ Property](dotnetimages/Property.gif) | [FlowPressureFile](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~FlowPressureFile.html) | Gets or sets the SOLIDWORKS Flow Simulation results file from which to import fluid pressure loads. |
| ![ Property](dotnetimages/Property.gif) | [FlowTemperatureFile](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~FlowTemperatureFile.html) | Gets or sets the SOLIDWORKS Flow Simulation results file from which to import flow temperatures. |
| ![ Property](dotnetimages/Property.gif) | [FrictionCoefficient](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~FrictionCoefficient.html) | Gets or sets the value of the coefficient of friction. |
| ![ Property](dotnetimages/Property.gif) | [HAdaptiveAccuracyBias](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveAccuracyBias.html) | Gets or sets the accuracy bias for the h-adaptive mesh iteration. |
| ![ Property](dotnetimages/Property.gif) | [HAdaptiveMaxNoIterations](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveMaxNoIterations.html) | Gets or sets the maximum number of h-adaptive mesh iterations. |
| ![ Property](dotnetimages/Property.gif) | [HAdaptiveMeshCoarsening](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveMeshCoarsening.html) | Obsolete. Superseded by [ICWStaticStudyOptions::HAdaptiveMeshCoarsening2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveMeshCoarsening2.html). |
| ![ Property](dotnetimages/Property.gif) | [HAdaptiveMeshCoarsening2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveMeshCoarsening2.html) | Gets or sets whether to allow h-adaptive mesh coarsening. |
| ![ Property](dotnetimages/Property.gif) | [HAdaptiveTargetAccuracy](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~HAdaptiveTargetAccuracy.html) | Gets or sets the target accuracy of the h-adaptive mesh iteration. |
| ![ Property](dotnetimages/Property.gif) | [IgnoreClearanceForSurfaceContact](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IgnoreClearanceForSurfaceContact.html) | Obsolete. Superseded by [ICWStaticStudyOptions::IgnoreClearanceForSurfaceContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IgnoreClearanceForSurfaceContact2.html). |
| ![ Property](dotnetimages/Property.gif) | [IgnoreClearanceForSurfaceContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IgnoreClearanceForSurfaceContact2.html) | Gets or sets whether to consider contact conditions regardless of the initial distance between user-defined face pairs. |
| ![ Property](dotnetimages/Property.gif) | [IncludeGlobalFriction](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IncludeGlobalFriction.html) | Obsolete. Superseded by [ICWStaticStudyOptions::IncludeGlobalFriction2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IncludeGlobalFriction2.html). |
| ![ Property](dotnetimages/Property.gif) | [IncludeGlobalFriction2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IncludeGlobalFriction2.html) | Gets or sets whether to include global friction. |
| ![ Property](dotnetimages/Property.gif) | [IncludeRemarkInReport](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IncludeRemarkInReport.html) | Obsolete. Superseded by [ICWStaticStudyOptions::IncludeRemarkInReport2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IncludeRemarkInReport2.html). |
| ![ Property](dotnetimages/Property.gif) | [IncludeRemarkInReport2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IncludeRemarkInReport2.html) | Gets or sets whether to include a remark in the report. |
| ![ Property](dotnetimages/Property.gif) | [IncompatibleBondingOption](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IncompatibleBondingOption.html) | Gets or sets the incompatible bonding option. |
| ![ Property](dotnetimages/Property.gif) | [LargeDisplacement](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~LargeDisplacement.html) | Obsolete. Superseded by [ICWStaticStudyOptions::LargeDisplacement2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~LargeDisplacement2.html). |
| ![ Property](dotnetimages/Property.gif) | [LargeDisplacement2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~LargeDisplacement2.html) | Gets or sets whether loads are applied gradually and uniformly in steps up to their full values, performing contact iterations at every step. |
| ![ Property](dotnetimages/Property.gif) | [NoPenetration](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~NoPenetration.html) | Obsolete. Superseded by [ICWStaticStudyOptions::NoPenetration2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~LargeDisplacement2.html). |
| ![ Property](dotnetimages/Property.gif) | [NoPenetration2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~NoPenetration2.html) | Gets or sets whether to improve accuracy for no penetration contacting surfaces. |
| ![ Property](dotnetimages/Property.gif) | [PAdaptiveConvergenceCriteria](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveConvergenceCriteria.html) | Gets or sets the criterion with which to determine convergence of the p-adaptive mesh iteration. |
| ![ Property](dotnetimages/Property.gif) | [PAdaptiveErrorLimit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveErrorLimit.html) | Gets or sets the highest percent change in [ICWStaticStudyOptions::PAdaptiveConvergenceCriteria](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveConvergenceCriteria.html) at which to end the p-adaptive mesh iteration. |
| ![ Property](dotnetimages/Property.gif) | [PAdaptiveMaxIterations](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveMaxIterations.html) | Gets or sets the maximum number of p-adaptive mesh iterations. |
| ![ Property](dotnetimages/Property.gif) | [PAdaptiveMaxPOrder](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveMaxPOrder.html) | Gets or sets the maximum polynomial order of the mesh at which to end the p-adaptive mesh iteration. |
| ![ Property](dotnetimages/Property.gif) | [PAdaptiveStartingPOrder](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveStartingPOrder.html) | Gets or sets the polynomial order at which to start the p-adaptive mesh iteration. |
| ![ Property](dotnetimages/Property.gif) | [PAdaptiveStrainEnergyErrorLimit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~PAdaptiveStrainEnergyErrorLimit.html) | Gets or sets the lowest relative strain energy error percent in model areas for which to apply a p-adaptive mesh iteration. |
| ![ Property](dotnetimages/Property.gif) | [ReferencePressureOption](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~ReferencePressureOption.html) | Gets or sets whether to use the reference pressure offset defined in the Flow Simulation results file to subtract from imported pressure values. |
| ![ Property](dotnetimages/Property.gif) | [RemarkComment](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~RemarkComment.html) | Gets or sets a report remark. |
| ![ Property](dotnetimages/Property.gif) | [ResultFolder](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~ResultFolder.html) | Gets or sets the path name of the folder that stores the results of the study. |
| ![ Property](dotnetimages/Property.gif) | [SolverType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~SolverType.html) | Gets or sets the solver type associated with the study. |
| ![ Property](dotnetimages/Property.gif) | [ThermalResults](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~ThermalResults.html) | Gets or sets the source of temperatures in this static study. |
| ![ Property](dotnetimages/Property.gif) | [ThermalStudyName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~ThermalStudyName.html) | Gets or sets the thermal study from which to import temperature values for this static study. |
| ![ Property](dotnetimages/Property.gif) | [TimeStep](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~TimeStep.html) | Gets or sets the time step at which to import a single temperature from a transient thermal study. |
| ![ Property](dotnetimages/Property.gif) | [UseInertialRelief](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~UseInertialRelief.html) | Obsolete. Superseded by [ICWStaticStudyOptions::UseInertialRelief2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~UseInertialRelief2.html). |
| ![ Property](dotnetimages/Property.gif) | [UseInertialRelief2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~UseInertialRelief2.html) | Gets or sets whether to solve using inertial relief. |
| ![ Property](dotnetimages/Property.gif) | [UseInPlaneEffect](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~UseInPlaneEffect.html) | Obsolete. Superseded by [ICWStaticStudyOptions::UseInPlaneEffect2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~UseInPlaneEffect2.html). |
| ![ Property](dotnetimages/Property.gif) | [UseInPlaneEffect2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~UseInPlaneEffect2.html) | Gets or sets whether to solve using inplane effect. |
| ![ Property](dotnetimages/Property.gif) | [UseSoftSpring](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~UseSoftSpring.html) | Obsolete. Superseded by [ICWStaticStudyOptions::UseSoftSpring2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~UseSoftSpring2.html). |
| ![ Property](dotnetimages/Property.gif) | [UseSoftSpring2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~UseSoftSpring2.html) | Gets or sets whether to solve using a soft spring to stabilize the model. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetZeroStrainTemperature](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~GetZeroStrainTemperature.html) | Gets the temperature at zero strain and its units. |
| ![ Method](dotnetimages/Method.gif) | [SetZeroStrainTemperature](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~SetZeroStrainTemperature.html) | Sets the temperature at zero strain and its units. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStaticStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)