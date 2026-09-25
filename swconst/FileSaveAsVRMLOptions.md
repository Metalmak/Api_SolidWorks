<!-- source: swconst/FileSaveAsVRMLOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > VRML

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture corresponds to the settings
  on that dialog.
* titled
  [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on the dialog but are now obsolete.

To display the dialog:

Click **Tools > Options > System Options > Export >
VRML** in **File Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **VRML**.
3. Click **Options**.

![](FileSaveAsVRMLOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Output as - Version | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportVrmlVersion)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportVrmlVersion, swVrmlOutputVersion\_e.<Value>) | Values as defined in swVrmlOutputVersion\_e |  |
| Output as - Unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportVrmlUnits)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportVrmlUnits, swLengthUnit\_e.<Value>) | Any of the following swLengthUnit\_e values:   * 0 = swMM (millimeters) * 1 = swCM (centimeters) * 2 = swMETER * 3 = swINCHES * 4 = swFEET |  |
| Save all components of the assembly in a single file | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swExportVrmlAllComponentsInSingleFile)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swExportVrmlAllComponentsInSingleFile, <OnFlag>) | Boolean value | Specifies whether to save all of the components of an assembly to a single VRML (.wrl) file |

Obsolete Enumerators

| Enumerator | Comment |
| swFileSaveAsCoordinateSystem | Obsolete |