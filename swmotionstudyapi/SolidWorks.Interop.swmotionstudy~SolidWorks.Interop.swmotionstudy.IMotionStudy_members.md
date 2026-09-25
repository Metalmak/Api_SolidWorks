<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| IMotionStudy Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) : IMotionStudy Interface |

The following tables list the members exposed by [IMotionStudy](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [IsActive](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~IsActive.html) | Gets whether this motion study is active. |
| ![ Property](dotnetimages/Property.gif) | [IsPlaying](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~IsPlaying.html) | Gets whether this motion study is playing. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~Name.html) | Gets or sets the name of a motion study. |
| ![ Property](dotnetimages/Property.gif) | [PlayMode](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~PlayMode.html) | Gets the mode in which this motion study is playing or sets the mode in which to play this motion study. |
| ![ Property](dotnetimages/Property.gif) | [StudyType](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~StudyType.html) | Gets or sets the type of this study. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [Activate](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~Activate.html) | Activates this motion study. |
| ![ Method](dotnetimages/Method.gif) | [Calculate](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~Calculate.html) | Performs the calculation for this motion study. |
| ![ Method](dotnetimages/Method.gif) | [CreateByCollapse](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateByCollapse.html) | Creates an animation in which an exploded view of an assembly is collapsed. |
| ![ Method](dotnetimages/Method.gif) | [CreateByExplode](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateByExplode.html) | Creates an animation in which a collapsed view of an assembly is exploded. |
| ![ Method](dotnetimages/Method.gif) | [CreateByRotateModel](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateByRotateModel.html) | Creates an animation that rotates the model. |
| ![ Method](dotnetimages/Method.gif) | [CreateDefinition](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateDefinition.html) | Creates the definition for the simulation feature data object. |
| ![ Method](dotnetimages/Method.gif) | [CreateFeature](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateFeature.html) | Creates a simulation feature using its feature data object. |
| ![ Method](dotnetimages/Method.gif) | [Duplicate](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~Duplicate.html) | Creates a new motion study based on the specified motion study. |
| ![ Method](dotnetimages/Method.gif) | [GetDuration](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetDuration.html) | Gets the duration, in seconds, of the motion study. |
| ![ Method](dotnetimages/Method.gif) | [GetFireOutputTimeStepEvents](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetFireOutputTimeStepEvents.html) | Gets whether output time step change events are fired at output time steps or integrator time steps. |
| ![ Method](dotnetimages/Method.gif) | [GetMotionFeatures](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetMotionFeatures.html) | Gets the motion features in this motion study. |
| ![ Method](dotnetimages/Method.gif) | [GetMotionFeaturesCount](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetMotionFeaturesCount.html) | Gets the number of motion features in this motion study. |
| ![ Method](dotnetimages/Method.gif) | [GetNumOfExternalForces](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetNumOfExternalForces.html) | Gets the numer of external forces in this motion study. |
| ![ Method](dotnetimages/Method.gif) | [GetNumOfExternalMotors](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetNumOfExternalMotors.html) | Gets the number of external motors in this motion study. |
| ![ Method](dotnetimages/Method.gif) | [GetProperties](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetProperties.html) | Gets the properties object for the specified type of motion study. |
| ![ Method](dotnetimages/Method.gif) | [GetResults](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetResults.html) | Gets the results object for the specified type of motion study. |
| ![ Method](dotnetimages/Method.gif) | [GetSupportedStudyTypes](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetSupportedStudyTypes.html) | Gets the types of studies supported by this motion study. |
| ![ Method](dotnetimages/Method.gif) | [GetTime](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~GetTime.html) | Gets the time, in seconds, where the timebar is on the timeline for this motion study. |
| ![ Method](dotnetimages/Method.gif) | [IGetMotionFeatures](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~IGetMotionFeatures.html) | Gets the motion features in this motion study. |
| ![ Method](dotnetimages/Method.gif) | [Play](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~Play.html) | Plays the animation; the start point is where the animation timebar is located. |
| ![ Method](dotnetimages/Method.gif) | [PlayFromStart](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~PlayFromStart.html) | Plays this motion study from the beginning. |
| ![ Method](dotnetimages/Method.gif) | [SaveToAVI](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~SaveToAVI.html) | Saves the animation to a .avi, .bmp, or .tga file. |
| ![ Method](dotnetimages/Method.gif) | [SetDuration](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~SetDuration.html) | Sets the duration, in seconds, of this motion study. |
| ![ Method](dotnetimages/Method.gif) | [SetFireOutputTimeStepEvents](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~SetFireOutputTimeStepEvents.html) | Sets whether output time step change events are fired at output time steps or integrator time steps. |
| ![ Method](dotnetimages/Method.gif) | [SetTime](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~SetTime.html) | Sets the time, in seconds, where to place the timebar on the timeline for this motion study. |
| ![ Method](dotnetimages/Method.gif) | [Stop](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~Stop.html) | Stops the currently playing animation. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IMotionStudy Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html)

[SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html)

[IMotionStudyManager Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager.html)

[IMotionStudyProperties Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyProperties.html)

[IMotionStudyResults Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyResults.html)