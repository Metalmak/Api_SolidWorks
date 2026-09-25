<!-- source: swconst/DP_Mates.htm -->

# SOLIDWORKS API Help

# Document Properties > Mates

![](DP_Mates.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Misaligned mates - Maximum deviation | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swMatesMaximumDeviationForMisalignedMates, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swMatesMaximumDeviationForMisalignedMates, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value | Valid only for assemblies |
| Misaligned mates - Default misalignment | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swMatesDefaultMisalignedType, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swMatesDefaultMisalignedType, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swMatesDefaultMisalignment\_e.<Value>) | Valid values as defined in swMatesDefaultMisalignment\_e | Valid only for assemblies |