<!-- source: swconst/FileSaveAsParasolidOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > Parasolid

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture corresponds to the
  settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on the dialog but are now obsolete.

To display the dialog:

Click **Tools > Options > System Options > Export > Parasolid** in **File
Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **Parasolid** or **Parasolid
   Binary**.
3. Click **Options**.

![](FileSaveAsParasolidOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Output as - Version | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swParasolidOutputVersion)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swParasolidOutputVersion, swParasolidOutputVersion\_e.<Value>) | See swParasolidOutputVersion\_e for valid options |  |
| Flatten assembly hierarchy | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swXTAssemSaveFormat)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swXTAssemSaveFormat, <OnFlag>) | Boolean value | Specifies whether to flatten assembly hierarchy in Parasolid output; for assemblies only |

Obsolete Enumerators

| Enumerator | Comment |
| swFileSaveAsCoordinateSystem | Obsolete |