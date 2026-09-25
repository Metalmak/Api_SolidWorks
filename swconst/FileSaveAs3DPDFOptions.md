<!-- source: swconst/FileSaveAs3DPDFOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > 3DPDF

To display the dialog:

Click **Tools > Options > System Options > Export >
3DPDF** in **File Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **Adobe Portable Document Format**.
3. Select **Save as 3D PDF**.
4. Click **Options**.

![](FileSaveAs3DPDFOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| Accuracy - Maximum, High, Medium, or Low | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.sw3DPDFAccuracy)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.sw3DPDFAccuracy, sw3DPDFAccuracy\_e.<Value>) | See sw3DPDFAccuracy\_e for valid options |  |
| Use lossy compression on tessellation | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.sw3DPDFCompressLossyTessellation)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.sw3DPDFCompressLossyTessellation, <OnFlag>) | Boolean value | Specifies whether to use lossy compression on tessellation |