<!-- source: swconst/FileSaveAsParasolidSheetMetalOptions.htm -->

# SOLIDWORKS API Help

# File > Save As > Save as type > Parasolid or Parasolid Binary > Save > Export

![](FileSaveAsParasolidSMExportOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Export sheet metal part in flattened mode | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPartExportFlatPattern)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPartExportFlatPattern, <OnFlag>) | Boolean value | Specifies whether to a export sheet metal part in flattened mode or not; for sheet metal parts only |