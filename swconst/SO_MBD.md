<!-- source: swconst/SO_MBD.htm -->

# SOLIDWORKS API Help

# System Options > MBD

The following MBD settings are not supported in SOLIDWORKS Connected.

![](SO_MBD.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Allow editing of Templates for 3DPDF's (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdit3DPDFTemplate)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdit3DPDFTemplate, <OnFlag>) | Boolean value |  |