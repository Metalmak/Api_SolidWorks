<!-- source: swconst/FilePageSetupPrintLineThickness.htm -->

# SOLIDWORKS API Help

# File > Print > Line Thickness

Getting and setting system-level line thicknesses for a printer using
the following enumerators are obsolete and superseded by [document-level
enumerators](DP_LineThickness.htm).

IMPORTANT: In SOLIDWORKS 2009
and later, SOLIDWORKS recommends that you set document-level line weights
instead of system-level line weights. However, if you must set system-level
line weights on a document created in SOLIDWORKS 2008 or earlier, then
you must set the system-level line weights before opening the document.

| Enumerator | Get/Set Methods | Return Value  or  <Value> | Comment |
| swPageSetupPrinterThinLineWeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThinLineWeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThinLineWeight, <Value>) | Double value in meters | Obsolete; specified  weight of thin line setting |
| swPageSetupPrinterNormalLineWeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterNormalLineWeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterNormalLineWeight, <Value>) | Double value in meters | Obsolete; specified  weight of normal line setting |
| swPageSetupPrinterThickLineWeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThickLineWeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThickLineWeight, <Value>) | Double value in meters | Obsolete; specified  weight of first thick line setting |
| swPageSetupPrinterThick2LineWeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick2LineWeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick2LineWeight, <Value>) | Double value in meters | Obsolete; specified  weight of second thick line setting |
| swPageSetupPrinterThick3LineWeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick3LineWeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick3LineWeight, <Value>) | Double value in meters | Obsolete; specified  weight of third thick line setting |
| swPageSetupPrinterThick4LineWeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick4LineWeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick4LineWeight, <Value>) | Double value in meters | Obsolete; specified  weight of fourth thick line setting |
| swPageSetupPrinterThick5LineWeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick5LineWeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick5LineWeight, <Value>) | Double value in meters | Obsolete; specified  weight of fifth thick line setting |
| swPageSetupPrinterThick6LineWeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick6LineWeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swPageSetupPrinterThick6LineWeight, <Value>) | Double value in meters | Obsolete; specified  weight of sixth thick line setting |