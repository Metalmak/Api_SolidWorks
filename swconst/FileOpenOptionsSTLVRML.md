<!-- source: swconst/FileOpenOptionsSTLVRML.htm -->

# SOLIDWORKS API Help

# System Options > Import > STL/OBJ/OFF/PLY/PLY2

To display the dialog:

Click **Tools > Options > System Options > Import > STL/OBJ/OFF/PLY/PLY2**
in **File Format**.

- or -

1. Click **File > Open**.
2. In **Files of type**, select
   **Mesh Files**.
3. Click **Options**.

![](FileOpenOptionsSTLVRML.gif)

| Setting | Get/Set Methods | Return Value  or   <Value>  or  <OnFlag> | Comment |
| Import as - Graphics body | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportStlVrmlModelType) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportStlVrmlModelType, swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Graphics) | swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Graphics |  |
| Import as - Solid body | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportStlVrmlModelType) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportStlVrmlModelType, swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Solid) | swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Solid |  |
| Import as - Surface body | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportStlVrmlModelType) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportStlVrmlModelType, swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Surface) | swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Surface |  |
| Mesh body options - Create mesh bodies bounded by single faces | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swVrmlStlImportAsPSMesh)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swVrmlStlImportAsPSMesh, <OnFlag>) | Boolean value | Valid only when importing as Solid body or Surface body, specifies whether to create mesh bodies bounded by single faces |
| Mesh body options - Group facets into faces | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIVrmlStlImportSegmented)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIVrmlStlImportSegmented, <OnFlag>) | Boolean value | Valid only if **Create mesh bodies bounded by single faces** is selected, specified whether to group facets into faces |
| Unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportStlVrmlUnits) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportStlVrmlUnits, swLengthUnit\_e.<Value>) | Valid options from swLengthUnit\_e:   * 0 = swMM (millimeters) * 1 = swCM (centimeters) * 2 = swMETER * 3 = swINCHES * 4 = swFEET |  |