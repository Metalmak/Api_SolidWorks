<!-- source: swconst/DP_Annotations-RevisionClouds.htm -->

S

# SOLIDWORKS API Help

# Document Properties > Annotations > Revision Clouds

![](DP_Annotations-RevisionClouds.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Overall drafting standard | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimensionStandard, swUserPreferenceOption\_e.swDetailingRevisionCloud)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimensionStandard, swUserPreferenceOption\_e.swDetailingRevisionCloud, swDetailingStandard\_e.<Value>) | See swDetailingStandard\_e for valid options | Specifies the overall drafting standard |
| Line style - Frame Style | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingRevisionCloudLineStyle, swUserPreferenceOption\_e.swDetailingRevisionCloud)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingRevisionCloudLineStyle, swUserPreferenceOption\_e.swDetailingRevisionCloud, swLineStyles\_e.<Value>) | See swLineStyles\_e for valid options | Specifies the style of the frames of revision clouds |
| Line style - Frame Thickness | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingRevisionCloudLineThickness, swUserPreferenceOption\_e.swDetailingRevisionCloud)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingRevisionCloudLineThickness, swUserPreferenceOption\_e.swDetailingRevisionCloud, swLineWeights\_e.<Value>) | See swLineWeights\_e for valid options | Specifies the thickness of the frames of revision clouds |
| Line style - Custom Thickness | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingRevisionCloudLineThicknessCustom, swUserPreferenceOption\_e.swDetailingRevisionCloud)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingRevisionCloudLineThicknessCustom, swUserPreferenceOption\_e.swDetailingRevisionCloud, <Value>) | Double value | Specifies a custom thickness for the frames of revision clouds; sets **Custom Thickness** to the specified thickness and **Frame Thickness** to **Custom Size** |
| Maximum arc radius | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingRevisionCloudMaxArcRadius, swUserPreferenceOption\_e.swDetailingRevisionCloud)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingRevisionCloudMaxArcRadius, swUserPreferenceOption\_e.swDetailingRevisionCloud, <Value>) | Double value | Specifies the maximum radius of each frame arc |
| Layer | IModelDocExtension::GetUserPreferenceString(swUserPreferenceStringValue\_e.swDetailingLayer, swUserPreferenceOption\_e.swDetailingRevisionCloud)  IModelDocExtension::SetUserPreferenceString(swUserPreferenceStringValue\_e.swDetailingLayer, swUserPreferenceOption\_e.swDetailingRevisionCloud, <Value>) | Valid Options:   * "Border" * "Dimensions" * "Notes" * "BOM" * "FORMAT" | This setting is available only on drawings; depending on drawing, some options may not apply |