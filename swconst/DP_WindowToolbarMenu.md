<!-- source: swconst/DP_WindowToolbarMenu.htm -->

# SOLIDWORKS API Help

# Window > Viewport

 ![](DP_toolbar_window_menu.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comment |
| Four View | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swFourViewportProjectionType, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swFourViewportProjectionType, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value> | Boolean value | Specifies whether to view the model or drawing in four viewports |