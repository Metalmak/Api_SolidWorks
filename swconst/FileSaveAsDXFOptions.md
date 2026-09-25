<!-- source: swconst/FileSaveAsDXFOptions.htm -->

# SOLIDWORKS API Help

# File > Save As > Save as type > Dxf or Dwg > Options

In order to display this dialog, open a part or drawing and:

Click **Tools > Options > System Options > Export >
DXF/DWG**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **Dxf or Dwg**.
3. Click **Options**.

This topic contains four tables. The information in the table:

* appearing immediately after the screen capture corresponds to the
  settings on that dialog.
* titled **[Hidden Layers Dialog Enumerators](#HiddenLayers)**
  contains enumerators corresponding to options on the hidden layers warning
  dialog that pops up during export to DXF/DWG of drawings that have one or
  more hidden layers.
* titled [Miscellaneous
  Enumerators](#Miscellaneous) contains miscellaneous DXF/DWG enumerators.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on the
  dialog but are now obsolete.

![](FileSaveAsDXFOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Version | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfVersion) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfVersion, swDxfFormat.e.<Value>) | See swDxfFormat\_e for valid options |  |
| Fonts | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfOutputFonts) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfOutputFonts, swDxfFormat.e.<Value>) | * 0 = AutoCAD STANDARD only * 1 = TrueType |  |
| Line styles | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfOutputLineStyles) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfOutputLineStyles, swDxfFormat.e.<Value>) | * 0 = AutoCAD Standard Styles * 1 = SOLIDWORKS Custom Styles |  |
| Custom Map SOLIDWORKS to DXF/DWG - Enable | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfMapping)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfMapping, <OnFlag>) | Boolean value | Specifies whether to implement mapping |
| Custom Map SOLIDWORKS to DXF/DWG - Don't show mapping on each save | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDXFDontShowMap)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDXFDontShowMap, <OnFlag>) | Boolean value | Specifies whether dialog appears when saving drawing when swDxfMapping set to True |
| Custom Map SOLIDWORKS to DXF/DWG - Map file | ISldWorks::GetUserPreferenceStringListValue(swUserPreferenceStringListValue\_e.swDxfMappingFiles)  ISldWorks::SetUserPreferenceStringListValue(swUserPreferenceStringListValue\_e.swDxfMappingFiles, <Value>) **IMPORTANT**: In addition to specifying the custom map file, you must specify a custom map file index to indicate which custom map file to use in the custom map file list. The following code snippet shows how to specify the custom map file index when adding the first custom map file to the custom map file list: swApp.SetUserPreferenceStringListValue swUserPreferenceStringListValue\_e.swDxfMappingFiles, mapFilePath index = swApp.GetUserPreferenceIntegerValue (swUserPreferenceIntegerValue\_e.swDxfMappingFileIndex) If (index = -1) Then swApp.SetUserPreferenceIntegerValue swUserPreferenceIntegerValue\_e.swDxfMappingFileIndex, 0  End If index = swApp.GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfMappingFileIndex) result= swModel.SaveAs4(outputPath, swSaveAsVersion\_e.swSaveAsCurrentVersion, swSaveAsOptions\_e.swSaveAsOptions\_Silent, errors, warnings) | String value | Sets up DXF/DWG mapping file; setting is persistent across SOLIDWORKS sessions; you can also interactively get or set the custom map file setting by clicking File, Save As, .dxf or .dwg as Save as type, and Options; separate each string in the list by a line feed  (e.g., the vbLf constant in Visual Basic) |
| Scale output 1:1 - Enable and Base scale | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfOutputNoScale) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfOutputNoScale, <Value>) | * 0 = not enabled * 1 = 1:1 scale | Enabled for drawings only; no options currently available to either  differentiate between sheet scale and view scale or specify a scale factor |
| Scale output 1:1 - Warn me if enabled | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| End Point Merging - Enable Merging | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfEndPointMerge)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfEndPointMerge, <OnFlag>) | Boolean value | Specifies whether to merge the end points of entities when exporting a part  to a DXF/DWG file; this option helps to avoid gaps between model edges, but it increases the export time; it is off by default |
| End Point Merging - <n> | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDxfMergingDistance)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDxfMergingDistance, <Value>) | Double value | Specifies the tolerance within which gaps between line endpoints are eliminated |
| End Point Merging - High quality DWG export | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDXFHighQualityExport)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDXFHighQualityExport, <OnFlag>) | Boolean value | Only for End Point Merging - Enable Merging set to True; specifies whether to export at a higher level of quality (with a possible increase in time to export) |
| Spline export options - Export all splines as splines | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfExportSplinesAsSplines)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfExportSplinesAsSplines, <OnFlag>) | True | Specifies to export all splines as splines |
| Spline export options - Export all splines as polylines | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfExportSplinesAsSplines)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfExportSplinesAsSplines, <OnFlag>) | False | Specifies to export all splines as polylines |
| Multiple sheet drawing - Export active sheet only | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfMultiSheetOption) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfMultiSheetOption, swDxfMultiSheet\_e.swDxfActiveSheetOnly) | swDxfMultiSheet\_e.swDxfActiveSheetOnly | See swDxfMultiSheet\_efor all valid options |
| Multiple sheet drawing - Export all sheets to separate files | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfMultiSheetOption) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfMultiSheetOption, swDxfMultiSheet\_e.swDxfSeparateSheets) | swDxfMultiSheet\_e.swDxfSeparateSheets | See swDxfMultiSheet\_efor all valid options |
| Multiple sheet drawing - Export all sheets to one file | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfMultiSheetOption) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfMultiSheetOption, swDxfMultiSheet\_e.swDxfMultiSheet) | swDxfMultiSheet\_e.swDxfMultiSheet | See swDxfMultiSheet\_efor all valid options |
| Multiple sheet drawing - Export all drawing sheets to paper space | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfExportAllSheetsToPaperSpace)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfExportAllSheetsToPaperSpace, <OnFlag>) | Boolean | Specifies to export all sheets to paper space |

Hidden Layers Enumerators

![](FileSaveAsDXFHiddenLayersOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| Do you want to export entities on all layers? *<Yes/No>* | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDXFExportHiddenLayersOn)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDXFExportHiddenLayersOn, <OnFlag>) | Boolean value | Specifies whether to export layers that are hidden in the drawing |
| Do not ask again | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDXFExportHiddenLayersWarnIsOn)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDXFExportHiddenLayersWarnIsOn, <OnFlag>) | Boolean value | Specifies whether to dismiss the hidden layers warning dialog on export; restore the dismissed dialog in **System Options > Advanced** |

Miscellaneous Enumerators

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swDxfMappingFileIndex | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfMappingFileIndex) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDxfMappingFileIndex, <Value>) **IMPORTANT**: In addition to specifying the custom map file, you must specify a custom map file index to indicate which custom map file to use in the custom map file list. The following code snippet shows how to specify the custom map file index when adding the first custom map file to the custom map file list: swApp.SetUserPreferenceStringListValue \_    swDxfMappingFiles, mapFilePath index = swApp.GetUserPreferenceIntegerValue \_    swDxfMappingFileIndex) If (index = -1) Then swApp.SetUserPreferenceIntegerValue \_     swDxfMappingFileIndex, 0  End If result= swModel.SaveAs4(outputPath,\_     swSaveAsCurrentVersion, \_        swSaveAsOptions\_Silent, errors, warnings) | Integer value | Specifies a custom map file index to indicate which custom map file to use in the custom map file list; index into list of custom map files or -1 |
| swDxfUseSolidworksLayers | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfUseSolidworksLayers)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDxfUseSolidworksLayers, <OnFlag>) | Boolean value | Specifies whether to apply the mapping file settings only to those entities whose layers are not defined and to preserve existing SOLIDWORKS drawing file layers in the exported file or to have the mapping file definitions overwrite all of the current SOLIDWORKS drawing file layers; this enumerator is equivalent to the Keep existing SOLIDWORKS drawing layer for entities option in the SOLIDWORKS to DXF/DWG Mapping dialog |

Obsolete Enumerators

| Enumerator | Get/Set Method | Return Value  or  <Value> | Comment |
| swDxfOutputScaleFactor | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDxfOutputScaleFactor)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDxfOutputScaleFactor, <Value>) | Double value | Specifies value to scale DXF output |