<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWFatigueStudyOptions Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWFatigueStudyOptions Interface |

The following tables list the members exposed by [ICWFatigueStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [ComputingAlternatingStressOption](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ComputingAlternatingStressOption.html) | Gets or sets the stress type used to calculate alternating stress. |
| ![ Property](dotnetimages/Property.gif) | [ConstantAmplitudeEventInteractionOption](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ConstantAmplitudeEventInteractionOption.html) | Gets or sets the interaction between constant amplitude fatigue events. |
| ![ Property](dotnetimages/Property.gif) | [EMail](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMail.html) | Obsolete. Superseded by [ICWFatigueStudyOptions::Email2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMail2.html). |
| ![ Property](dotnetimages/Property.gif) | [EMail2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMail2.html) | Gets or sets whether to email notifications during simulations. |
| ![ Property](dotnetimages/Property.gif) | [EMailInterval](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMailInterval.html) | Gets or sets the time interval for sending email notifications during simulations. |
| ![ Property](dotnetimages/Property.gif) | [EMailIntervalUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMailIntervalUnit.html) | Gets or sets the units of time for [ICWFatigueStudyOptions::EMailInterval](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMailInterval.html). |
| ![ Property](dotnetimages/Property.gif) | [EMailTimebased](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMailTimebased.html) | Obsolete. Superseded by [ICWFatigueStudyOptions::EmailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMailTimebased2.html). |
| ![ Property](dotnetimages/Property.gif) | [EMailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMailTimebased2.html) | Gets or sets whether to send email notifications during simulations. |
| ![ Property](dotnetimages/Property.gif) | [EMailTo](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMailTo.html) | Gets or sets the recipient of email notifications. |
| ![ Property](dotnetimages/Property.gif) | [FatigueStrengthReductionFactor](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~FatigueStrengthReductionFactor.html) | Gets or sets the fatigue strength reduction factor to use when reading S-N curve data. |
| ![ Property](dotnetimages/Property.gif) | [LoadingEventCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~LoadingEventCount.html) | Gets the number of loading events in the fatigue study. |
| ![ Property](dotnetimages/Property.gif) | [MeanStressCorrectionOption](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~MeanStressCorrectionOption.html) | Gets or sets the mean stress correction method to use in calculating alternating stresses. |
| ![ Property](dotnetimages/Property.gif) | [RandomVibrationComputationalMethod](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~RandomVibrationComputationalMethod.html) | Gets or sets the random vibration computational method. |
| ![ Property](dotnetimages/Property.gif) | [ResultFolder](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ResultFolder.html) | Gets or sets the folder for the results of the fatigue study. |
| ![ Property](dotnetimages/Property.gif) | [ShellFace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ShellFace.html) | Gets or sets the shell face on which fatigue analysis is performed. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddFatigueEventForConstantAmplitude](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForConstantAmplitude.html) | Adds a fatigue event to a linear dynamic constant amplitude study. |
| ![ Method](dotnetimages/Method.gif) | [AddFatigueEventForHarmonic](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForHarmonic.html) | Adds a fatigue event to a linear dynamic harmonic study. |
| ![ Method](dotnetimages/Method.gif) | [AddFatigueEventForRandomVibration](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForRandomVibration.html) | Adds a fatigue event to a linear dynamic random vibration study. |
| ![ Method](dotnetimages/Method.gif) | [AddFatigueEventForVariableAmplitude](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForVariableAmplitude.html) | Adds a fatigue event to a linear dynamic variable amplitude study. |
| ![ Method](dotnetimages/Method.gif) | [DeleteFatigueEvent](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~DeleteFatigueEvent.html) | Deletes the specified fatigue event. |
| ![ Method](dotnetimages/Method.gif) | [GetFatigueEvent](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~GetFatigueEvent.html) | Gets the specified fatigue event. |
| ![ Method](dotnetimages/Method.gif) | [GetInfiniteLifeSettings](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~GetInfiniteLifeSettings.html) | Obsolete. Superseded by [ICWFatigueStudyOptions::GetInfiniteLifeSettings2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~GetInfiniteLifeSettings2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetInfiniteLifeSettings2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~GetInfiniteLifeSettings2.html) | Gets the infinite life settings of the fatigue study. |
| ![ Method](dotnetimages/Method.gif) | [GetVariableAmplitudeEventOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~GetVariableAmplitudeEventOptions.html) | Gets the options for variable amplitude fatigue events. |
| ![ Method](dotnetimages/Method.gif) | [SetInfiniteLifeSettings](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~SetInfiniteLifeSettings.html) | Obsolete. Superseded by [ICWFatigueStudyOptions::SetInfiniteLifeSettings2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~SetInfiniteLifeSettings2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetInfiniteLifeSettings2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~SetInfiniteLifeSettings2.html) | Sets the infinite life settings of the fatigue study. |
| ![ Method](dotnetimages/Method.gif) | [SetVariableAmplitudeEventOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~SetVariableAmplitudeEventOptions.html) | Sets the options for variable amplitude fatigue events. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWFatigueStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)