<!-- source: swconst/DP_ColorsAdvanced.htm -->

# SOLIDWORKS API Help

# Document Properties > Colors > Advanced Properties

The Advanced Properties dialog appears when you click Advanced...
in Document Properties > Colors.  The
Advanced... button is enabled
only when Shading is selected in the Model/feature
colors combo box.

![](DP_ColorsAdvanced.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Ambient | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedAmbient, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedAmbient, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0 and 1 | Specifies how light is reflected and scattered by other objects |
| Diffuse | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedDiffuse, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedDiffuse, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0 and 1 | Specifies how light is scattered equally in all directions on the surface |
| Specularity | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedSpecularity, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedSpecularity, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0 and 1 | Specifies how surfaces exhibit highlights |
| Shininess | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedShininess, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedShininess, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0 and 1 | Specifies how solid objects alternate between a glossy, reflective surface and a dull, matte surface |
| Transparency | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedTransparency, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedTransparency, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0 and 1 | Specifies how much light passes through the surface |
| Emission | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedEmission, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDocumentColorAdvancedEmission, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0 and 1 | Specifies how light projects from the surface |