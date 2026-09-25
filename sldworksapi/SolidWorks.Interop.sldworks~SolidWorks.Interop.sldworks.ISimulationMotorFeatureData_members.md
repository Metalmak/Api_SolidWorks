<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISimulationMotorFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISimulationMotorFeatureData Interface |

The following tables list the members exposed by [ISimulationMotorFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [DirectionReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~DirectionReference.html) | Gets or sets the direction in which the motor moves. |
| ![ Property](dotnetimages/Property.gif) | [DriveType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~DriveType.html) | Sets the drive type of this motor feature. |
| ![ Property](dotnetimages/Property.gif) | [Expression](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~Expression.html) | Gets or sets the motor motion expression for this motor feature. |
| ![ Property](dotnetimages/Property.gif) | [ExternalState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~ExternalState.html) | Gets or sets whether your application can listen to motor-related motion study event. |
| ![ Property](dotnetimages/Property.gif) | [InterpolationScheme](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~InterpolationScheme.html) | Gets or set the interpolation scheme for this motor feature. |
| ![ Property](dotnetimages/Property.gif) | [LoadReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~LoadReferences.html) | Gets or sets the load references for this motor feature. |
| ![ Property](dotnetimages/Property.gif) | [Location](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~Location.html) | Select a face, vertex, or edge on the assembly for the reference origin when setting motion relative to another part. |
| ![ Property](dotnetimages/Property.gif) | [Magnitude](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~Magnitude.html) | Get or set the magnitude for this motor feature. |
| ![ Property](dotnetimages/Property.gif) | [MotionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~MotionType.html) | Gets or sets the type of motion of this motor feature. |
| ![ Property](dotnetimages/Property.gif) | [MotorType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~MotorType.html) | Gets the type of motor for this motor feature. |
| ![ Property](dotnetimages/Property.gif) | [RelativeComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~RelativeComponent.html) | Gets or sets a part in the assembly to which to reference motion when setting motion relative to another part in this motor feature. |
| ![ Property](dotnetimages/Property.gif) | [ReverseDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~ReverseDirection.html) | Gets or sets whether or not to reverse the direction of the motor. |
| ![ Property](dotnetimages/Property.gif) | [SplineData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~SplineData.html) | Gets or sets the spline data points for this motor feature. |
| ![ Property](dotnetimages/Property.gif) | [Velocity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~Velocity.html) | Gets or sets the speed of the motor if no other force acts on it. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [ConstantSpeedMotor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~ConstantSpeedMotor.html) | Sets the constant speed for this motor feature. |
| ![ Method](dotnetimages/Method.gif) | [DistanceMotor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~DistanceMotor.html) | Sets the distance and time for which to operate this motor feature. |
| ![ Method](dotnetimages/Method.gif) | [GetInterpolatedValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~GetInterpolatedValue.html) | Gets the interopolated value at the specified time for this motor feature. |
| ![ Method](dotnetimages/Method.gif) | [InterpolatedMotor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~InterpolatedMotor.html) | Sets the drive type and interpolation scheme for this motor feature. |
| ![ Method](dotnetimages/Method.gif) | [LoadSplineData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~LoadSplineData.html) | Loads the spline data from the specified file for this motor feature. |
| ![ Method](dotnetimages/Method.gif) | [OscillatingMotor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData~OscillatingMotor.html) | Sets the displacement and frequency for oscillating motion for this motor feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISimulationMotorFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ISimulationGravityFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationGravityFeatureData.html)

[Simulation3DContactFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation3DContactFeatureData.html)

[SimulationDamperFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationDamperFeatureData.html)

[SimulationForceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData.html)

[ISimulationSpringFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationSpringFeatureData.html)