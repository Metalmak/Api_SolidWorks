<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| SolidWorks.Interop.swmotionstudy Namespace | |
| [See Also](#seealsobookmark)  [Inheritance Hierarchy](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace_hierarchy.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

SOLIDWORKS Motion Study API

# ![](dotnetimages/collapse.gif)Interfaces

| Interface | Description |
| --- | --- |
| [IAVIParameter](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IAVIParameter.html) | Allows access to the parameters of a file containing an animation. |
| [ICosmosMotionStudyProperties](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties.html) | Allows access to a motion study's properties. |
| [ICosmosMotionStudyResults](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyResults.html) | Allows access to a motion study's results. |
| [IMotionPlotFeatureOutput](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionPlotFeatureOutput.html) | Allows access to a plot's values. |
| [IMotionStudy](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html) | Allows access to a SOLIDWORKS motion study's results. |
| [IMotionStudyManager](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager.html) | Allows access to the MotionManager. |
| [IMotionStudyProperties](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyProperties.html) | Allows access to a SOLIDWORKS motion study's properties. |
| [IMotionStudyResults](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyResults.html) | Allows access to a SOLIDWORKS motion study's results. |
| [IPhysicalSimulationMotionStudyProperties](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IPhysicalSimulationMotionStudyProperties.html) | Allows access to a Physical Simulation motion study's properties. |

# ![](dotnetimages/collapse.gif)Delegates

| Delegate | Description |
| --- | --- |
| [DMotionStudyEvents\_ForceOutputTimeStepChangeNotifyEventHandler](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_ForceOutputTimeStepChangeNotifyEventHandler.html) | Fired at every integrator or output time step when a motion simulation is occurring and external forces exist. |
| [DMotionStudyEvents\_ForceTimeStepChangeNotifyEventHandler](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_ForceTimeStepChangeNotifyEventHandler.html) | Fired when a motion study is [calculated](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.IMotionStudy~Calculate.html) and there are external forces. |
| [DMotionStudyEvents\_MotorOutputTimeStepChangeNotifyEventHandler](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_MotorOutputTimeStepChangeNotifyEventHandler.html) | Fired at every integrator or output time step when a motion simulation is occurring and external motors exist. |
| [DMotionStudyEvents\_MotorTimeStepChangeNotifyEventHandler](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_MotorTimeStepChangeNotifyEventHandler.html) | Fired when a motion study is [calculated](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.IMotionStudy~Calculate.html) and there are external motors. |
| [DMotionStudyEvents\_OutputTimeStepChangeNotifyEventHandler](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_OutputTimeStepChangeNotifyEventHandler.html) | Fired at every integrator or output time step when a motion simulation is occurring. |
| [DMotionStudyEvents\_PartCollideNotifyEventHandler](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_PartCollideNotifyEventHandler.html) | Fired when a collision between two components occurs. |
| [DMotionStudyEvents\_SpecialMotionEventNotifyEventHandler](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_SpecialMotionEventNotifyEventHandler.html) | Fired for motion-related special events, such as contacts. |
| [DMotionStudyEvents\_StartCalculateNotifyEventHandler](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_StartCalculateNotifyEventHandler.html) | Fired when a motion study is [calculated](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.IMotionStudy~Calculate.html). |
| [DMotionStudyEvents\_StopCalculateNotifyEventHandler](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_StopCalculateNotifyEventHandler.html) | Fired when a motion study's calculation ends. |

# ![](dotnetimages/collapse.gif)Enumerations

| Enumeration | Description |
| --- | --- |
| [swMotionIntegratorType\_e](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.swMotionIntegratorType_e.html) | Integration methods for solving numerically stiff systems. |
| [swMotionStudyNotify\_e](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.swMotionStudyNotify_e.html) | To receive notifications, a DLL application must register for the notifications by object type. This registration must be done for each instance of a particular object. |
| [swMotionStudyType\_e](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.swMotionStudyType_e.html) | Motion study types. Bitmask. |
| [swSaveAVIImageSize\_e](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.swSaveAVIImageSize_e.html) | AVI image sizes. |
| [swSpecialMotionEventType\_e](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.swSpecialMotionEventType_e.html) | Motion-related special events. |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swmotionstudy Assembly](SolidWorks.Interop.swmotionstudy.html)