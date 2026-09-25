<!-- source: swconst/FilePageSetup.htm -->

# SOLIDWORKS API Help

# File > Page Setup

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture
  of the Page Setup dialog corresponds to the settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on
  the Page Setup dialog, but are now obsolete and no longer appear on that
  dialog.

![](FilePageSetup.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Use system settings | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Use this document settings | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Set each drawing sheet individually | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Settings for | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Scale and Resolution  - Scale to fit | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupDrawingScaleToFit) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupDrawingScaleToFit, <OnFlag>) | Boolean value | Specifies whether to print drawing sheet to fit paper size; for drawings only; Use system settings on Page Setup dialog must be selected when changing this setting. |
| Scale and Resolution - Scale | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Scale and Resolution - <n> | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Scale and Resolution - High Quality | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupHighQuality) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupHighQuality, <OnFlag>) | Boolean value | Specifies whether to load all model information into memory; for drawings only |
| Scale and Resolution - Scale draft edges | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupScaleDraftEdges) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupScaleDraftEdges, <OnFlag>) | Boolean value | Specifies whether to scale draft edges; for drawings only |
| Drawing Color - Automatic | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupDrawingColor)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupDrawingColor, swPageSetupDrawingColor\_e.swPageSetup\_AutomaticDrawingColor) | swPageSetupDrawingColor\_e.swPageSetup\_AutomaticDrawingColor | See swPageSetupDrawingColor\_efor all valid options |
| Drawing Color - Color / Gray scale | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupDrawingColor)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupDrawingColor, swPageSetupDrawingColor\_e.swPageSetup\_ColorGrey) | swPageSetupDrawingColor\_e.swPageSetup\_ColorGrey) | See swPageSetupDrawingColor\_efor all valid options |
| Drawing Color - Black and white | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupDrawingColor)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupDrawingColor, swPageSetupDrawingColor\_e.swPageSetup\_BlackAndWhite) | swPageSetupDrawingColor\_e.swPageSetup\_BlackAndWhite) | See swPageSetupDrawingColor\_efor all valid options |
| Paper - Size | See Comment | See Comment | Defined by the operating system or by a specific printer device; there is no SOLIDWORKS API enumeration for these values |
| Paper - Source | See Comment | See Comment | Defined by the operating system or by a specific printer device; there is no SOLIDWORKS API enumeration for these values |
| Orientation - Portrait | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupPrinterOrientation)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupPrinterOrientation, swPageSetupOrientation\_e.swPageSetupOrient\_Portrait) | swPageSetupOrientation\_e.swPageSetupOrient\_Portrait | See swPageSetupOrientation\_e for all valid options |
| Orientation - Landscape | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupPrinterOrientation)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPageSetupPrinterOrientation, swPageSetupOrientation\_e.swPageSetupOrient\_Landscape) | swPageSetupOrientation\_e.swPageSetupOrient\_Landsacpe | See swPageSetupOrientation\_e for all valid options |

Obsolete
Enumerators

| Enumerator | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| swPageSetupPrinterPartAsmPrintWindow | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupPrinterPartAsmPrintWindow) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupPrinterPartAsmPrintWindow, <OnFlag>) | Boolean value | Obsolete; for parts and assemblies only; specified whether to print current view of the graphics area; Use system settings on Page Setup dialog must be selected when changing this setting |
| swPageSetupDrawingScale | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e, swPageSetupDrawingScale)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e, swPageSetupDrawingScale, <Value>) | Double value | Obsolete |
| swPageSetupPrinterPartAsmScale | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e, swPageSetupPrinterPartAsmScale)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e, swPageSetupPrinterPartAsmScale, <Value>) | Double value | Obsolete |