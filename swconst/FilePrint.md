<!-- source: swconst/FilePrint.htm -->

# SOLIDWORKS API Help

# File > Print

![](FilePrint.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Name | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Document Options - Header/Footer | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Document Options - Line Thickness | See Comment | See Comment | See [Document Properties > Line Thickness](DP_LineThickness.htm) |
| System Options - Margins | See Comment | See Comment | See [File > Page Setup > Print > System Options > Margins](FilePageSetupPrintSystemOptionsMargins.htm) |
| Print range - Entire model | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Print range - Current sheet | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Print range - Current screen image | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Print range - Sheets | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Print range - Sheets - <n> | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Number of copies <n> | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Print background | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPrintBackground) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPrintBackground, <OnFlag>) | Boolean value | Specifies whether to print the window background, in addition to the model and drawing |
| Print to file | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Convert draft quality drawing views to high quality | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Print cross hatch on out of date views | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Print white lines, text in black | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Print grid | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPrintGrid) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPrintGrid, <OnFlag>) | Boolean value | Specifies whether to print the grid |
| Print zone lines | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPrintZoneLines) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPrintZoneLines, <OnFlag>) | Boolean value | Specifies whether to print zone lines |