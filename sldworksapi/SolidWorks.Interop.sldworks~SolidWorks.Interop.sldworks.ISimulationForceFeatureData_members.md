<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISimulationForceFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISimulationForceFeatureData Interface |

The following tables list the members exposed by [ISimulationForceFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [ActionDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ActionDirection.html) | Gets or sets the direction of the force. |
| ![ Property](dotnetimages/Property.gif) | [ActionLocation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ActionLocation.html) | Gets or sets the location at which to apply the force for an action-only force. |
| ![ Property](dotnetimages/Property.gif) | [ActionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ActionType.html) | Gets or sets the type of action for this Force feature. |
| ![ Property](dotnetimages/Property.gif) | [ExternalState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ExternalState.html) | Gets or sets whether your application can listen to force-related motion study events. |
| ![ Property](dotnetimages/Property.gif) | [ForceFunctionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ForceFunctionType.html) | Gets or sets the type of function for this Force feature. |
| ![ Property](dotnetimages/Property.gif) | [ForceType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ForceType.html) | Gets the type of force.  **NOTE: This property is a get-only property. Set is not implemented.** |
| ![ Property](dotnetimages/Property.gif) | [FunctionConstantValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~FunctionConstantValue.html) | Gets or sets the function constant value for this Force feature. |
| ![ Property](dotnetimages/Property.gif) | [FunctionExpression](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~FunctionExpression.html) | Gets or sets the expression function for this Force feature. |
| ![ Property](dotnetimages/Property.gif) | [FunctionInterpolatedValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~FunctionInterpolatedValues.html) | Gets or sets the interpolated values for this Force feature. |
| ![ Property](dotnetimages/Property.gif) | [InterpolationScheme](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~InterpolationScheme.html) | Gets the interopolation scheme for this Force feature. |
| ![ Property](dotnetimages/Property.gif) | [LoadReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~LoadReferences.html) | Gets or sets the load references for this Force feature. |
| ![ Property](dotnetimages/Property.gif) | [ReactionLocation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ReactionLocation.html) | Gets or sets the location at which to apply the force for an action/reaction force. |
| ![ Property](dotnetimages/Property.gif) | [ReferenceComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ReferenceComponent.html) | Gets or sets the component to serve as a reference frame for the force. |
| ![ Property](dotnetimages/Property.gif) | [ReverseDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ReverseDirection.html) | Gets or sets whether to reverse the direction of the force. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetEndPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~GetEndPoints.html) | Gets the end points of this Force feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFunctionHarmonicValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~GetFunctionHarmonicValues.html) | Gets the harmonic function values for this Force feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFunctionStepValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~GetFunctionStepValues.html) | Gets the step function, whose magnitude transitions smoothly from one value to another value, for this Force feature. |
| ![ Method](dotnetimages/Method.gif) | [GetInterpolatedValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~GetInterpolatedValue.html) | Gets the interpolated value at the specified time for this Force feature. |
| ![ Method](dotnetimages/Method.gif) | [LoadSplineData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~LoadSplineData.html) | Loads the spline data from the specified file for this Force feature. |
| ![ Method](dotnetimages/Method.gif) | [SetEndPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~SetEndPoints.html) | Sets the end points for this Force feature. |
| ![ Method](dotnetimages/Method.gif) | [SetFunctionHarmonicValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~SetFunctionHarmonicValues.html) | Sets the harmonic function values for this Force feature. |
| ![ Method](dotnetimages/Method.gif) | [SetFunctionStepValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~SetFunctionStepValues.html) | Sets the step function, whose magnitude transitions smoothly from one value to another value, for this Force feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISimulationForceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ISimulationGravityFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationGravityFeatureData.html)

[ISimulationMotorFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData.html)

[Simulation3DContactFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation3DContactFeatureData.html)

[SimulationDamperFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationDamperFeatureData.html)

[ISimulationSpringFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationSpringFeatureData.html)