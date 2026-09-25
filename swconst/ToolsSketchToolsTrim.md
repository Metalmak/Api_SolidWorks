<!-- source: swconst/ToolsSketchToolsTrim.htm -->

# SOLIDWORKS API Help

# Tools > Sketch Tools > Trim

![](ToolsSketchToolsTrim.gif)

| Setting | Get/Set Methods | Return Value   or  <OnFlag> | **Comments** |
| Keep trimmed entities as construction geometry | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swMakeTrimEntityConstruction)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swMakeTrimEntityConstruction, <OnFlag>) | Boolean value |  |
| Ignore trimming of construction geometry | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIgnoreConstructionEntity)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIgnoreConstructionEntity, <OnFlag>) | Boolean value |  |