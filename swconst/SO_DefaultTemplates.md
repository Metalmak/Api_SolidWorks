<!-- source: swconst/SO_DefaultTemplates.htm -->

# SOLIDWORKS API Help

# System Options > Default Templates

![](SO_DefaultTemplates.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Parts | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swDefaultTemplatePart)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swDefaultTemplatePart, <Value>) | String value |  |
| Assemblies | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swDefaultTemplateAssembly)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swDefaultTemplateAssembly, <Value>) | String value |  |
| Drawings | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swDefaultTemplateDrawing)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swDefaultTemplateDrawing, <Value>) | String value |  |
| Always use these default document templates | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAlwaysUseDefaultTemplates)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAlwaysUseDefaultTemplates, <OnFlag>) | True | Specifies whether to use default template or prompt for name of template |
| Prompt user to select document template | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAlwaysUseDefaultTemplates)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAlwaysUseDefaultTemplates, <OnFlag>) | False | Specifies whether to prompt for name of template |