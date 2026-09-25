<!-- source: swconst/ToolsCompSelectIdenticalCompMatchConfig.htm -->

# SOLIDWORKS API Help

# Tools > Component Selection > Select Identical Components

![](ToolsCompSelectIdenticalCompMatchConfig.gif)

| Setting | Get/Set Methods | Return Value   or  <OnFlag> | **Comments** |
| Options - Match configuration names | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swMatchConfigurationNames)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swMatchConfigurationNames, <OnFlag>) | Boolean value | Specifies whether to match configuration names; valid only for assemblies |