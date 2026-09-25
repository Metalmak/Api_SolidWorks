<!-- source: swconst/FileSaveAs.htm -->

# SOLIDWORKS API Help

# File > Save As

![](FileSaveAsPartWithoutCostingData.gif)

![](FileSaveAsPartFrmAsmOptions.gif)

![](FileSaveAsIFC.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Save without Costing data | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSaveWithoutCostingData)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSaveWithoutCostingData, <OnFlag>) | Boolean value | Specifies whether to save the sheet metal part without any Costing data |
| Geometry to save:  * Exterior faces * Exterior components * All components | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSaveAssemblyAsPartOptions) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSaveAssemblyAsPartOptions, swSaveAsmAsPartOptions\_e.<Value>) | See swSaveAsmAsPartOptions\_e for valid options | Specifies the geometry of an assembly to save as a multi-body part |
| Preserve geometry references | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSaveAsmAsPartPreserveIDs)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSaveAsmAsPartPreserveIDs, <OnFlag>) | Boolean value | Specifies whether to preserve geometry reference IDs when saving an assembly as a part |
| Save as type - IFC 2x3 or IFC 4 | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSaveIFCFormat)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSaveIFCFormat, <Value>) | * 23   = IFC 2x3 * 4 = IFC 4 | Specifies the IFC format in which to save a part |