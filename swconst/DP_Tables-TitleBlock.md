<!-- source: swconst/DP_Tables-TitleBlock.htm -->

# SOLIDWORKS API Help

# Document Properties > Tables > Title Block

![](DP_Tables-TitleBlock.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Border - Box Border | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingTitleBlockTableBorderLineWeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingTitleBlockTableBorderLineWeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swLineWeights\_e.<Value>) | See swLineWeights\_e for valid options | For assemblies and parts only. |
| Border - Grid Border | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingTitleBlockTableGridLineWeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingTitleBlockTableGridLineWeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swLineWeights\_e.<Value>) | See swLineWeights\_e for valid options | For assemblies and parts only. |
| Text - Font... | IModelDocExtension::GetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingTitleBlockTableTextFormat, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingTitleBlockTableTextFormat, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | See ITextFormat for font options | To set font property values, implement ITextFormat, set the appropriate ITextFormat member values, and pass the ITextFormat object in the API set method. For assemblies and parts only. |