<!-- source: swconst/DP_MaterialProperties.htm -->

# SOLIDWORKS API Help

# Document Properties > Material Properties

![](DP_MaterialProperties.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Density | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swMaterialPropertyDensity, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swMaterialPropertyDensity, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value in kg/m^3 | For parts only; specifies material density |
| Area Hatch/Fill - Style | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swMaterialPropertyAreaHatchFillStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swMaterialPropertyAreaHatchFillStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swAreaHatchFillStyle\_e.<Value>) | See swAreaHatchFillStyle\_e for valid options |  |
| Area Hatch/Fill - Pattern | IModelDocExtension::GetUserPreferenceString(swUserPreferenceStringValue\_e.swMaterialPropertyCrosshatchPattern, swuserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceString(swUserPreferenceStringValue\_e.swMaterialPropertyCrosshatchPattern, swuserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Valid string values:  ![](SO_Drawings-areaHatchFillPattern.gif) | For parts only; for hatch style only |
| Area Hatch/Fill - Scale | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swMaterialPropertyCrosshatchScale, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swMaterialPropertyCrosshatchScale, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value | For parts only; for hatch style only; specifies value by which to scale crosshatch |
| Area Hatch/Fill - Angle | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swMaterialPropertyCrosshatchAngle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swMaterialPropertyCrosshatchAngle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value | For parts only; for hatch style only; specifies angle for crosshatch |