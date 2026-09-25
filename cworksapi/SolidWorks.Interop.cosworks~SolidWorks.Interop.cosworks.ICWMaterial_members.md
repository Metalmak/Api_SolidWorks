<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWMaterial Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWMaterial Interface |

The following tables list the members exposed by [ICWMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Category](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~Category.html) | Gets or sets the category of the material. |
| ![ Property](dotnetimages/Property.gif) | [Count](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~Count.html) | Gets the number of properties defined for this material. |
| ![ Property](dotnetimages/Property.gif) | [Description](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~Description.html) | Gets or sets the description for the material. |
| ![ Property](dotnetimages/Property.gif) | [IncludeCreep](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~IncludeCreep.html) | Obsolete. Superseded by [ICWMaterial::IncludeCreep2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~IncludeCreep2.html). |
| ![ Property](dotnetimages/Property.gif) | [IncludeCreep2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~IncludeCreep2.html) | Gets or sets whether to include creep effect for the material model in nonlinear studies only. |
| ![ Property](dotnetimages/Property.gif) | [MaterialName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~MaterialName.html) | Gets or sets the name of the material name. |
| ![ Property](dotnetimages/Property.gif) | [MaterialUnits](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~MaterialUnits.html) | Gets or sets the units for the material. |
| ![ Property](dotnetimages/Property.gif) | [ModelType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~ModelType.html) | Gets or sets the material model. |
| ![ Property](dotnetimages/Property.gif) | [MooneyRivlinConstants](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~MooneyRivlinConstants.html) | Gets or sets the Mooney Rivlin constants for the MooneyRivlin material model used in nonlinear studies only. |
| ![ Property](dotnetimages/Property.gif) | [NoOfBulkModuli](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~NoOfBulkModuli.html) | Gets or sets the number of bulk moduli for the viscoelastic material model used in nonlinear studies only. |
| ![ Property](dotnetimages/Property.gif) | [NoOfShearModuli](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~NoOfShearModuli.html) | Gets or sets the number of shear moduli for the viscoelastic material model used in nonlinear studies only. |
| ![ Property](dotnetimages/Property.gif) | [OgdenConstants](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~OgdenConstants.html) | Gets or sets the Ogden constants used for the Ogden material model used for nonlinear studies only. |
| ![ Property](dotnetimages/Property.gif) | [SNCurveEstimateConstants](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SNCurveEstimateConstants.html) | Gets or sets whether to specify the Basquin Equation constants, B and slope (m), or let the program calculate them from the S-N curve. |
| ![ Property](dotnetimages/Property.gif) | [SNCurveEstimateCutoff](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SNCurveEstimateCutoff.html) | Gets or sets the cut-off point for estimating Basquin Eqation constants, B and slope (m). |
| ![ Property](dotnetimages/Property.gif) | [SNCurveSlopeM](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SNCurveSlopeM.html) | Gets or sets the slope (m) of the S-N curve. |
| ![ Property](dotnetimages/Property.gif) | [SNCurveSource](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SNCurveSource.html) | Gets or sets the source for the material S-N curve used in fatigue studies. |
| ![ Property](dotnetimages/Property.gif) | [SNCurveSpecificConstantB](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SNCurveSpecificConstantB.html) | Gets or sets the B constant of the Basquin Equation. |
| ![ Property](dotnetimages/Property.gif) | [SNCurveSpecificConstantBUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SNCurveSpecificConstantBUnit.html) | Gets or sets the units of the Basquin Equation constants. |
| ![ Property](dotnetimages/Property.gif) | [Source](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~Source.html) | Returns the source of the material. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetAustenticSteelCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetAustenticSteelCurve.html) | Gets the austentic steel curve data. |
| ![ Method](dotnetimages/Method.gif) | [GetCarbonSteelCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetCarbonSteelCurve.html) | Gets the carbon steel curve data. |
| ![ Method](dotnetimages/Method.gif) | [GetFatigueSNCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetFatigueSNCurve.html) | Gets the fatigue S-N curve data for user-defined curve sources. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialDataCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetMaterialDataCurve.html) | Obsolete. Superseded by [ICWMaterial::GetMaterialDataCurve3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetMaterialDataCurve3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialDataCurve3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetMaterialDataCurve3.html) | Gets the material data curve. |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyByName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetPropertyByName.html) | Obsolete. Superseded by er[ICWMaterial::GetPropertyByName2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetPropertyByName2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyByName2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetPropertyByName2.html) | Gets the value of the material property by the property name. |
| ![ Method](dotnetimages/Method.gif) | [GetReferencePlaneName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetReferencePlaneName.html) | Gets the name of the reference plane or reference axis used to specify material properties for orthotropic materials. |
| ![ Method](dotnetimages/Method.gif) | [GetStressStrainCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetStressStrainCurve.html) | Gets the stress strain curve data. |
| ![ Method](dotnetimages/Method.gif) | [GetTemperatureCurveForProperty](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetTemperatureCurveForProperty.html) | Gets the temperature curve data for the material property. |
| ![ Method](dotnetimages/Method.gif) | [SetFatigueSNCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetFatigueSNCurve.html) | Sets the fatigue S-N curve data for user-defined curve sources. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialDataCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetMaterialDataCurve.html) | Obsolete. Superseded by [ICWMaterial::SetMaterialDataCurve3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetMaterialDataCurve3.html). |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialDataCurve3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetMaterialDataCurve3.html) | Sets the material data curve. |
| ![ Method](dotnetimages/Method.gif) | [SetPropertyByName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetPropertyByName.html) | Obsolete. Superseded by [ICWMaterial::SetPropertyByName2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetPropertyByName2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetPropertyByName2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetPropertyByName2.html) | Sets the value of the specified material property. |
| ![ Method](dotnetimages/Method.gif) | [SetReferencePlane](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetReferencePlane.html) | Sets the name of the reference plane or reference axis used to specify material properties for orthotropic materials. |
| ![ Method](dotnetimages/Method.gif) | [SetStressStrainCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetStressStrainCurve.html) | Sets the stress-strain curve data. |
| ![ Method](dotnetimages/Method.gif) | [SetTemperatureCurveForProperty](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetTemperatureCurveForProperty.html) | Sets the temperature curve data for the material property. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWShell Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell.html)

[ICWSolidBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html)

[ICWBeamBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html)