<!-- source: swconst/ToolsSketchEntitiesRectangle.htm -->

# SOLIDWORKS API Help

# Tools > Sketch Entities > Corner Rectangle or Center Rectangle or 3 Point Corner Rectangle or 3 Point Center Rectangle or Parallelogram

![](ToolsSketchEntitiesRectangle.gif)

| Setting | Get/Set Methods | Return Value   or  <OnFlag> | **Comments** |
| Rectangle Type - Add construction lines - From Corner | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSketchAddConstLineDiagonalType)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSketchAddConstLineDiagonalType, <OnFlag>) | Boolean value | Specifies whether to add construction lines from the corners |
| Rectangle Type - Add construction lines - From Midpoint | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSketchAddConstToRectEntity)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSketchAddConstToRectEntity, <OnFlag>) | Boolean value | Specifies whether to add construction lines from the midpoint |