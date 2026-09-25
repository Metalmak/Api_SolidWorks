<!-- source: swconst/ViewModifyQuickViewTransparency.htm -->

# SOLIDWORKS API Help

# View > Modify > Filter Modified Components

![](ViewModifyQuickViewTransparency.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Transparency level - Enable | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickViewTransparencyEnabled)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickViewTransparencyEnabled, <OnFlag>) | Boolean value | Specifies whether to activate the transparency for unmodified components of assemblies opened in Large Design Review |
| Transparency level - Dynamic | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickViewTransparencyDynamic)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickViewTransparencyDynamic, <OnFlag>) | Boolean value | Specifies whether to update the transparency level in the graphics area when the slider is moved in the Transparency Level PropertyManager page |
| Transparency level - Level ranges from 0 to 1 | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swQuickViewTransparencyLevel)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swQuickViewTransparencyLevel, <Value>) | Double value | Specifies the value to which to adjust the transparency for unmodified components in assemblies opened in Large Design Review |