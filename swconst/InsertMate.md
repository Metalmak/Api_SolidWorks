<!-- source: swconst/InsertMate.htm -->

# SOLIDWORKS API Help

# Insert > Mate (*assemblies only*)

![](InsertMate.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Options - Make first selection transparent | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swMakeFirstSelectionTransparentInMateDialog, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swMakeFirstSelectionTransparentInMateDialog, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to make the first mate selection transparent |