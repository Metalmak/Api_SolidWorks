<!-- source: sldworksapi/Display_Shadows_in_Shaded_Mode_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Display Shadow Example

This example shows how to turn on shadows using swDisplayShadowsInShadedMode,
which is a system setting.

iSldWorks->SetUserPreferenceToggle(swDisplayShadowsInShadedMode,
TRUE);

pInputDoc->GraphicsRedraw2();