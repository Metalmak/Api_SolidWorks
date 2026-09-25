<!-- source: swconst/FileOpenOptionsSLDXML.htm -->

# SOLIDWORKS API Help

# File > Open > Files of type > SLDXML > Options

![](FileOpenOptionsSLDXML.gif)

| Setting | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| Import sketch data | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSLDXMLImportSketchData)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSLDXMLImportSketchData, <OnFlag>) | Boolean value | Specifies whether to import sketch data |
| Import sketch objects in a mechanism sketch as blocks | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSLDXMLImportMechanismSketchObjectsAsBlocks)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSLDXMLImportMechanismSketchObjectsAsBlocks, <OnFlag>) | Boolean value | Specifies whether to import sketch objects in a mechanism sketch as blocks; swImportSLDXMLImportSketchData must be true for this option to be applicable |
| Import assembly mates data | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSLDXMLImportAssemblyMatesData)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSLDXMLImportAssemblyMatesData, <OnFlag>) | Boolean value | Specifies whether to import assembly mates data |