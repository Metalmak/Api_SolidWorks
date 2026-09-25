<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWForce Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWForce Interface |

The following tables list the members exposed by [ICWForce](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Equation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~Equation.html) | Gets or sets the equation describing this force of nonuniform distribution. |
| ![ Property](dotnetimages/Property.gif) | [EquationAngularUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationAngularUnit.html) | Gets or sets the angular units for the cylindrical or spherical coordinate system of this force of nonuniform distribution. |
| ![ Property](dotnetimages/Property.gif) | [EquationCoordinateSystemType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationCoordinateSystemType.html) | Gets or sets the type of coordinate system used to define this force of nonuniform distribution. |
| ![ Property](dotnetimages/Property.gif) | [EquationLinearUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationLinearUnit.html) | Gets or sets the linear units for the Cartesian, cylindrical, or spherical coordinate system of this force of nonuniform distribution. |
| ![ Property](dotnetimages/Property.gif) | [ForceType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceType.html) | Gets or sets the force type. |
| ![ Property](dotnetimages/Property.gif) | [IncludeNonUniformDistribution](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~IncludeNonUniformDistribution.html) | Obsolete. Superseded by [ICWForce::IncludeNonUniformDistribution2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~IncludeNonUniformDistribution2.html). |
| ![ Property](dotnetimages/Property.gif) | [IncludeNonUniformDistribution2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~IncludeNonUniformDistribution2.html) | Gets or sets whether to use a nonuniform distribution of this force. |
| ![ Property](dotnetimages/Property.gif) | [NormalForceOrTorqueValue](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~NormalForceOrTorqueValue.html) | Gets or sets the normal or torque value of this force. |
| ![ Property](dotnetimages/Property.gif) | [PhaseAngle](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~PhaseAngle.html) | Gets or sets the phase angle of the force in a harmonic analysis of a linear dynamic study. |
| ![ Property](dotnetimages/Property.gif) | [PhaseAngleUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~PhaseAngleUnit.html) | Gets or sets the units of phase angle of the force in a harmonic analysis of a linear dynamic study. |
| ![ Property](dotnetimages/Property.gif) | [Unit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~Unit.html) | Gets or sets the units of force. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [ForceBeginEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceBeginEdit.html) | Starts editing a force. |
| ![ Method](dotnetimages/Method.gif) | [ForceEndEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceEndEdit.html) | Ends editing a force. |
| ![ Method](dotnetimages/Method.gif) | [GetCoordinateSystem](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetCoordinateSystem.html) | Gets the coordinate system used for defining a force of nonuniform distribution. |
| ![ Method](dotnetimages/Method.gif) | [GetForceComponentValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetForceComponentValues.html) | Obsolete. Superseded by [ICWForce::GetForceComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetForceComponentValues2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetForceComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetForceComponentValues2.html) | Gets the force component values. |
| ![ Method](dotnetimages/Method.gif) | [GetMomentComponentValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetMomentComponentValues.html) | Obsolete. Superseded by [ICWForce::GetMomentComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetMomentComponentValues2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetMomentComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetMomentComponentValues2.html) | Gets the moment values. |
| ![ Method](dotnetimages/Method.gif) | [GetNonUniformData](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetNonUniformData.html) | Obsolete. Superseded by [ICWForce::Equation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~Equation.html). |
| ![ Method](dotnetimages/Method.gif) | [GetTimeCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetTimeCurve.html) | Gets the time curve data for this time-dependent force in a dynamic study. |
| ![ Method](dotnetimages/Method.gif) | [InsertEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~InsertEntity.html) | Adds an entity to the set of entities to which to apply this force or torque. |
| ![ Method](dotnetimages/Method.gif) | [RemoveEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~RemoveEntity.html) | Removes an entity at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [SetCoordinateSystem](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetCoordinateSystem.html) | Sets the coordinate system used for defining a force of nonuniform distribution. |
| ![ Method](dotnetimages/Method.gif) | [SetForceComponentValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetForceComponentValues.html) | Obsolete. Superseded by [ICWForce::SetForceComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetForceComponentValues2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetForceComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetForceComponentValues2.html) | Sets the force component values. |
| ![ Method](dotnetimages/Method.gif) | [SetMomentComponentValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetMomentComponentValues.html) | Obsolete. Superseded by [ICWForce::SetMomentComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetMomentComponentValues2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetMomentComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetMomentComponentValues2.html) | Sets the moment values. |
| ![ Method](dotnetimages/Method.gif) | [SetNonUniformData](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetNonUniformData.html) | Obsolete. Superseded by [ICWForce::Equation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~Equation.html). |
| ![ Method](dotnetimages/Method.gif) | [SetReferenceGeometry](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetReferenceGeometry.html) | Sets the reference entity along whose direction this force is applied. |
| ![ Method](dotnetimages/Method.gif) | [SetTimeCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetTimeCurve.html) | Obsolete. Superseded by [ICWForce::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetTimeCurve2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetTimeCurve2.html) | Sets the time curve data for this time-dependent force in a dynamic study. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)