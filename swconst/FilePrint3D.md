<!-- source: swconst/FilePrint3D.htm -->

# SOLIDWORKS API Help

# File > Print3D

![](FilePrint3D.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Printer - Custom Printer - Width | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPrint3DBoxX)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPrint3DBoxX, <Value>) | Double value |  |
| Printer - Custom Printer - Depth | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPrint3DBoxY)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPrint3DBoxY, <Value>) | Double value |  |
| Printer - Custom Printer - Height | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPrint3DBoxZ)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPrint3DBoxZ, <Value>) | Double value |  |