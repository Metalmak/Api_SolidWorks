<!-- source: swconst/DP_VirtualSharps.htm -->

# SOLIDWORKS API Help

# Document Properties > Virtual Sharps

![](DP_VirtualSharps.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Virtual sharp style | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingVirtualSharpStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingVirtualSharpStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDetailingVirtualSharp\_e.<Value>) | See swDetailingVirtualSharp\_e for valid options | Specifies display options for virtual sharps |