<!-- source: swconst/ToolsEvaluateMassProperties.htm -->

# SOLIDWORKS API Help

# Tools > Evaluate > Mass Properties

![](ToolsEvaluateMassProperties.gif)

| Setting | Get/Set Methods | Return Value   or  <OnFlag> | **Comments** |
| Options - Inertia Tensor (Crossproduct Convention) | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUsePositiveInertiaTensorNotation)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUsePositiveInertiaTensorNotation, <OnFlag>) | Boolean value | True for Positive Tensor Notation; false for Negative Tensor Notation |