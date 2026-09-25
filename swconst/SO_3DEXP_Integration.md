<!-- source: swconst/SO_3DEXP_Integration.htm -->

# SOLIDWORKS API Help

# System Options > 3DEXPERIENCE Integration

This dialog is only available in SOLIDWORKS Connected.

![](3DEXP_Integration.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Update SOLIDWORKS files for compatibility with the **3D**EXPERIENCE platform | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnable3DEXPERIENCEFileCompatibilityUpdate) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnable3DEXPERIENCEFileCompatibilityUpdate, <OnFlag>) | Boolean value | This option is enabled only when no documents are open |