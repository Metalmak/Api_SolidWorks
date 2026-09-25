<!-- source: swconst/DP_ViewLabels.htm -->

# SOLIDWORKS API Help

# Document Properties > Views

![](DP_ViewLabels.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Text - Font... | IModelDocExtension::GetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingViewTextFormat, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingViewTextFormat, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | See ITextFormat for font options | To set font property values, implement ITextFormat, set the appropriate ITextFormat member values, and pass the ITextFormat object in the API set method |