<!-- source: swconst/FileSaveAsIFCOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > IFC

This topic contains two tables. The information in the table:

* appearing immediately after the dialog corresponds to the settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on
  the dialog but are now obsolete.

To display the dialog:

Click **Tools > Options > System Options > Export > IFC** in **File
Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **IFC 2x3** or **IFC 4**.
3. Click **Options**.

![](FileSaveAsIFCOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Output as - OmniClass™ | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIFCOmniClassPreference)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIFCOmniClassPreference, <OnFlag>) | Boolean value |  |
| Output as - UniClass2 | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIFCUniClass2Preference)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIFCUniClass2Preference, <OnFlag>) | Boolean value |  |
| Output as - Custom Properties | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIFCCustomPropsPreference)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIFCCustomPropsPreference, <OnFlag>) | Boolean value |  |
| Output as - Material and Mass Properties | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIFCMaterialsMassPropertiesPreference)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIFCMaterialsMassPropertiesPreference, <OnFlag>) | Boolean value |  |
| Output as - Units | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportIFCUnits)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportIFCUnits, swLengthUnit\_e.<Value>) | Any of the following swLengthUnit\_e values:   * 0 = swMM (millimeters) * 1 = swCM (centimeters) * 2 = swMETER * 3 = swINCHES * 4 = swFEET |  |
| IFC4 Export - Save - BREP,  BREP and Tessellation, or Tessellation | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swIFCExportSaveType)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swIFCExportSaveType, swIFCExportSaveType\_e.<Value>) | See swIFCExportSaveType\_e for valid options |  |

Obsolete Enumerators

| Enumerator | Comment |
| swIFCOmniUniClassPreference | Obsolete |
| swExportIFCUniClass2 | Obsolete |
| swExportIFCType | Obsolete |