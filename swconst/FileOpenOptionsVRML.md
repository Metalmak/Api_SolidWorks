<!-- source: swconst/FileOpenOptionsVRML.htm -->

# SOLIDWORKS API Help

# System Options > Import > VRML or 3MF

To display the dialog:

Select **Tools > Options > System Options > Import > File Format
> VRML**
or **3MF**.

- or -

1. Select **File > Open**.
2. In **Files of type**, select
   **VRML** or **3D Manufacturing Format**.
3. Click **Options**.

![](FileOpenOptionsVRML.gif)

| Setting | Get/Set Methods | Return Value  or   <Value>  or  <OnFlag> | Comment |
| Import as - Graphics body | ISldWorks::GetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType) ISldWorks::SetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType, swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Graphics) | swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Graphics |  |
| Import as - Solid body | ISldWorks::GetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType) ISldWorks::SetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType, swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Solid) | swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Solid |  |
| Import as - Surface body | ISldWorks::GetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType) ISldWorks::SetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlModelType, swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Surface) | swImportStlVrmlModelType\_e.swImportStlVrmlModelType\_Surface |  |
| Unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlUnits) ISldWorks::SetUserPreferenceIntegerValue(swUserPerferenceIntegerValue\_e.swImportStlVrmlUnits, swLengthUnit\_e.<Value>) | Valid options from swLengthUnit\_e:   * 0 = swMM (millimeters) * 1 = swCM (centimeters) * 2 = swMETER * 3 = swINCHES * 4 = swFEET |  |
| Import texture information | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportStlVrmlTextureInformation)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportStlVrmlTextureInformation, <OnFlag>) | Boolean value |  |