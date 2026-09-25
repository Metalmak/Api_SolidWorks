<!-- source: swconst/FilePageSetupPrintSystemOptionsMargins.htm -->

# SOLIDWORKS API Help

# File > Print > Margins

![](FilePageSetupPrintSystemOptionsMargins.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Paper margins - Top | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterTopMargin)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterTopMargin, <Value>) | Double value in meters | Specifies width of left margin |
| Paper margins - Bottom | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterBottomMargin)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterBottomMargin, <Value>) | Double value in meters | Specifies width of left margin |
| Paper margins - Left | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterLeftMargin)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterLeftMargin, <Value>) | Double value in meters | Specifies width of left margin |
| Paper margins - Right | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterRightMargin)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterRightMargin, <Value>) | Double value in meters | Specifies width of left margin |
| Paper margins - Use printer's margins | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupPrinterUsePrinterMargin)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPageSetupPrinterUsePrinterMargin, <OnFlag>) | Boolean value | Specifies whether to print document with printer's default margin values |