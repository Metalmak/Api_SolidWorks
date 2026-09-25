<!-- source: swconst/FileSaveAsPartFrmAsmOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > SLDPRT from assembly

To display the dialog:

Click **Tools > Options > System Options > Export >
SLDPRT from assembly** in **File Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **Part (\*.prt, \*.sldprt)**.
3. Click **Options**.

![](FileSaveAsSLDPRTFrmAsmOptions.gif)

| Setting | Get/Set Methods | Return Value   or   <Value>   or   <OnFlag> | Comment |
| Specified components - Remove - Visibility threshold (internal components) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swASMSLDPRT\_ExcludeComponentsByVisibility)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swASMSLDPRT\_ExcludeComponentsByVisibility, <OnFlag>) | Boolean value | Specifies whether to remove from the export list those internal components whose visibility is less than the threshold specified by swASMSLDPRT\_ExcludeComponentsByVisibilityThreshold |
| Specified components - Remove - Visibility threshold (internal components) - (slider amount) | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swASMSLDPRT\_ExcludeComponentsByVisibilityThreshold)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swASMSLDPRT\_ExcludeComponentsByVisibilityThreshold, <Value>) | Double value in meters-cubed | Valid only if swASMSLDPRT\_ExcludeComponentsByVisibility is set to true |
| Specified components - Remove - Bounding box volume less than: | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swExcludeComponentsByBBoxVolume)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swExcludeComponentsByBBoxVolume, <OnFlag>) | Boolean value | Specifies whether to remove from the export list those components whose bounding box volumes are less than the threshold specified by swASMSLDPRT\_ExcludeComponentsByBBoxVolumeThreshold |
| Specified components - Remove - Bounding box volume less than: (amount) | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swASMSLDPRT\_ExcludeComponentsByBBoxVolumeThreshold)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swASMSLDPRT\_ExcludeComponentsByBBoxVolumeThreshold, <Value>) | Double value in meters-cubed | Valid only if swExcludeComponentsByBBoxVolume is set to true |
| Specified components - Remove - Fastener components | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swASMSLDPRT\_ExcludeIfToolboxComponents)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swASMSLDPRT\_ExcludeIfToolboxComponents, <OnFlag>) | Boolean value | Specifies whether to remove from the export list fastener components |
| Specified components - Include - Mass properties | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swASMSLDPRT\_IncludeMassProperties)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swASMSLDPRT\_IncludeMassProperties, <OnFlag>) | Boolean value | Specifies whether to override the mass properties of the part with the mass properties from the assembly |