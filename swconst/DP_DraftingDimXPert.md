<!-- source: swconst/DP_DraftingDimXPert.htm -->

# SOLIDWORKS API Help

# Document Properties > DimXpert

![](DP_DraftingDimXpert.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Chamfer dimension scheme | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimXpertChamferScheme, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimXpertChamferScheme, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDetailingDimXpertChamferStyle\_e.<Value>) | See swDetailingDimXpertChamferStyle\_e for valid options | Specifies chamfer dimension scheme |
| Slot dimension scheme | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimXpertSlotScheme, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimXpertSlotScheme, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDetailingDimXpertSlotStyle\_e.<Value>) | See swDetailingDimXpertSlotStyle\_e for valid options | Specifies slot dimension scheme |
| Fillet options | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimXpertFilletOptions, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimXpertFilletOptions, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDetailingDimXpertFilletInstanceStyle\_e.<Value>) | See swDetailingDimXpertFilletInstanceStyle\_e for valid options | Specifies fillet options |
| Chamfer options | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimXpertChamferOptions, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimXpertChamferOptions, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDetailingDimXpertChamferInstanceStyle\_e.<Value>) | See swDetailingDimXpertChamferInstanceStyle\_e for valid options | Specifies chamfer options |