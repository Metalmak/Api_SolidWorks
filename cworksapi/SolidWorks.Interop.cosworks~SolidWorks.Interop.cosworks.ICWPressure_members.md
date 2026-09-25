<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWPressure Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWPressure Interface |

The following tables list the members exposed by [ICWPressure](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CoordSystemType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~CoordSystemType.html) | Gets or sets the type of coordinate system used to define this nonuniform pressure. |
| ![ Property](dotnetimages/Property.gif) | [DirectionType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~DirectionType.html) | Gets or sets how this pressure is applied along the specified reference geometry. |
| ![ Property](dotnetimages/Property.gif) | [Equation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~Equation.html) | Gets or sets the equation describing this pressure of nonuniform distribution. |
| ![ Property](dotnetimages/Property.gif) | [EquationAngularUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~EquationAngularUnit.html) | Gets or sets the angular units for cylindrical and spherical coordinate systems of the nonuniform pressure distribution equation. |
| ![ Property](dotnetimages/Property.gif) | [EquationLinearUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~EquationLinearUnit.html) | Gets or sets the linear units for Cartesian, cylindrical, and spherical coordinate systems of the nonuniform pressure distribution equation. |
| ![ Property](dotnetimages/Property.gif) | [IncludeNonUniformDistribution](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~IncludeNonUniformDistribution.html) | Obsolete. Superseded by [ICWPressure::IncludeNonUniformDistribution2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~IncludeNonUniformDistribution2.html). |
| ![ Property](dotnetimages/Property.gif) | [IncludeNonUniformDistribution2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~IncludeNonUniformDistribution2.html) | Gets or sets whether to use a nonuniform distribution of pressure. |
| ![ Property](dotnetimages/Property.gif) | [PhaseAngle](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~PhaseAngle.html) | Gets or sets the phase angle of the pressure in a linear dynamic harmonic study. |
| ![ Property](dotnetimages/Property.gif) | [PhaseAngleUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~PhaseAngleUnit.html) | Gets or sets the units of phase angle of the pressure in a linear dynamic harmonic study. |
| ![ Property](dotnetimages/Property.gif) | [PressureType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~PressureType.html) | Gets or sets the pressure direction type (normal or use reference geometry). |
| ![ Property](dotnetimages/Property.gif) | [ReverseDirection](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~ReverseDirection.html) | Obsolete. Superseded by [ICWPressure::ReverseDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~ReverseDirection2.html). |
| ![ Property](dotnetimages/Property.gif) | [ReverseDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~ReverseDirection2.html) | Gets or sets whether to reverse the direction of this pressure. |
| ![ Property](dotnetimages/Property.gif) | [Unit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~Unit.html) | Gets or sets the units of pressure. |
| ![ Property](dotnetimages/Property.gif) | [Value](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~Value.html) | Gets or sets the pressure value. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetCoordinateSystem](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~GetCoordinateSystem.html) | Gets the coordinate system that defines this nonuniform pressure. |
| ![ Method](dotnetimages/Method.gif) | [GetNonUniformData](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~GetNonUniformData.html) | Obsolete. Superseded by [ICWPressure::Equation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~Equation.html). |
| ![ Method](dotnetimages/Method.gif) | [GetTimeCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~GetTimeCurve.html) | Gets the time curve data for this time-dependent pressure in a dynamic study. |
| ![ Method](dotnetimages/Method.gif) | [InsertEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~InsertEntity.html) | Inserts a face to which to apply this pressure. |
| ![ Method](dotnetimages/Method.gif) | [PressureBeginEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~PressureBeginEdit.html) | Starts editing pressure. |
| ![ Method](dotnetimages/Method.gif) | [PressureEndEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~PressureEndEdit.html) | Ends editing pressure. |
| ![ Method](dotnetimages/Method.gif) | [RemoveEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~RemoveEntity.html) | Removes the entity at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [SetCoordinateSystem](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetCoordinateSystem.html) | Sets the coordinate system that defines this nonuniform pressure. |
| ![ Method](dotnetimages/Method.gif) | [SetNonUniformData](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetNonUniformData.html) | Obsolete. Superseded by [ICWPressure::Equation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~Equation.html). |
| ![ Method](dotnetimages/Method.gif) | [SetReferenceGeometry](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetReferenceGeometry.html) | Sets the face, edge, plane, or axis to be used to set the direction of this pressure. |
| ![ Method](dotnetimages/Method.gif) | [SetTimeCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetTimeCurve.html) | Obsolete. Superseded by [ICWPressure::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetTimeCurve2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetTimeCurve2.html) | Sets the time curve data for this time-dependent pressure in a dynamic study. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)