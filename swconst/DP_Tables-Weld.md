<!-- source: swconst/DP_Tables-Weld.htm -->

# SOLIDWORKS API Help

# Document Properties > Tables > Weld

![](DP_Tables-Weld.gif)

**NOTE:** Setting any of the following weld
table values means that new weld tables added to the drawing use these default
values. However, a weld table that uses a template table for insertion might
not use these default values because the template table contains certain
properties that take precedence over these default values.

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Border - Box Border | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingWeldTableBorderLineWeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingWeldTableBorderLineWeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swLineWeights\_e.<Value>) | See swLineWeights\_e for valid options |  |
| Border - Grid Border | ModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingWeldTableGridLineWeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingWeldTableGridLineWeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swLineWeights\_e.<Value>) | See swLineWeights\_e for valid options |  |
| Text - Font... | IModelDocExtension::GetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingWeldSymbolTextFormat, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingWeldSymbolTextFormat, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | See ITextFormat for font options | To set font property values, implement ITextFormat, set the appropriate ITextFormat member values, and pass the ITextFormat object in the set method |
| Trailing zeroes | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimTrailingZero, swUserPreferenceOption\_e.swDetailingWeldTable)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimTrailingZero, swUserPreferenceOption\_e.swDetailingWeldTable, swDetailingDimTrailingZero\_e.<Value>) | Valid options in swDetailingDimTrailingZero\_e:  * swDimShowTrailingZeroes * swDimRemoveTrailingZeroes * swDimRemoveOnlyOnZero * swDimSameAsSource |  |
| Layer | IModelDocExtension::GetUserPreferenceString(swUserPreferenceStringValue\_e.swDetailingLayer, swUserPreferenceOption\_e.swDetailingWeldTable)  IModelDocExtension::SetUserPreferenceString(swUserPreferenceStringValue\_e.swDetailingLayer, swUserPreferenceOption\_e.swDetailingWeldTable, <Value>) | Valid options:   * "Border" * "Dimensions" * "Notes" * "BOM" * "FORMAT" * "None" | This setting is available only on drawings; depending on drawing, some options may not apply |