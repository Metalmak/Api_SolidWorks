<!-- source: swconst/DP_Tables.htm -->

# SOLIDWORKS API Help

# Document Properties > Tables

![](DP_Tables.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Text - Font... | IModelDocExtension::GetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingTableTextFormat, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingTableTextFormat, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | See ITextFormat for font options | To set font property values, implement ITextFormat, set the appropriate ITextFormat member values, and pass the ITextFormat object in the API set method |
| Use template settings | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingTablesUseTemplateSettings, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingTablesUseTemplateSettings, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to override a table's document properties with the settings of an imported template |
| Cell paddings - Horizontal padding | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingTablesHorizontalPadding, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingTablesHorizontalPadding, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value | Specifies the horizontal padding for table cells |
| Cell paddings - Vertical padding | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingTablesVerticalPadding, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingTablesVerticalPadding, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value | Specifies the vertical padding for table cells |