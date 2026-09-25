<!-- source: swconst/DP_DraftingStandard.htm -->

# SOLIDWORKS API Help

# Document Properties > Drafting Standard

![](DP_DraftingStandard.gif)

| Setting | Get/Set Methods | Return Value  or   <Value>  or  <OnFlag> | Comments |
| Overall drafting standard | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimensionStandard, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimensionStandard, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDetailingStandard\_e.<Value>) | See swDetailingStandard\_e for valid options | Specifies the base drafting standard to use |
| Uppercase - All uppercase for notes | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDraftingStandardUppercase, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDraftingStandardUppercase, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <OnFlag>) | Boolean value | Specifies whether to set the drafting standard to all uppercase for notes |
| Uppercase - All uppercase for tables | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDraftingStandardAllUppercaseForTable, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDraftingStandardAllUppercaseForTable, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <OnFlag>) | Boolean value | Specifies whether to set the drafting standard to all uppercase for tables |
| Uppercase - All uppercase for dimensions and hole callouts | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDraftingStandardAllUppercaseForDimensionsAndHoleCallouts, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDraftingStandardAllUppercaseForDimensionsAndHoleCallouts, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <OnFlag>) | Boolean value |  |
| Uppercase - Exclusion list | IModelDocExtension::GetUserPreferenceString(swUserPreferenceStringValue\_e.swDraftStandardExclusionList, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceString(swUserPreferenceStringValue\_e.swDraftStandardExclusionList, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | String value | Specifies the list of strings to exclude from making uppercase |