<!-- source: swconst/FileSaveAsPDFOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > PDF

To display the dialog:

Click **Tools > Options > System Options > Export >
PDF** in **File Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **Adobe Portable Document Format**.
3. Click **Options**.

![](FileSaveAsPDFOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| Export PDF in color | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportInColor)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportInColor, <OnFlag>) | Boolean value | Specifies whether to save documents in color when saving to PDF |
| Embed fonts | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportEmbedFonts)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportEmbedFonts, <OnFlag>) | Boolean value | Specifies whether to embed fonts when saving documents  to PDF |
| High quality lines | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportHighQuality)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportHighQuality, <OnFlag>) | Boolean value | Specifies whether to save drawing documents in high quality when saving to PDF |
| Shaded/Draft geometry DPI | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPDFExportShadedDraftDPI)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPDFExportShadedDraftDPI, <Value>) | Integer value | For drawings only; controls dots per inch (DPI) setting for shaded and draft geometry; increased value improves quality while increasing the file size and the time to save the file |
| Sharpened OLE DPI | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPDFExportOleDPI)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPDFExportOleDPI, <Value>) | Integer value | For drawings only; controls DPI setting for Object Linking and Embedding (OLE) objects; increased value improves quality while increasing the file size and the time to save the file |
| High quality shaded edges | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportShadedEdgesHighQuality)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportShadedEdgesHighQuality, <OnFlag>) | Boolean value |  |
| Print header/footer | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportPrintHeaderFooter)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportPrintHeaderFooter, <OnFlag>) | Boolean value | Specifies whether to use the header and footer specified in File > Print > Header Footer when saving documents to PDF |
| Use specified printer line weights (File > Print > Line Weights) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportUseCurrentPrintLineWeights)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportUseCurrentPrintLineWeights, <OnFlag>) | Boolean value | Specifies whether to use the default printer line weights when saving documents to PDF |
| Include layers set to not print | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportIncludeLayersNotToPrint)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportIncludeLayersNotToPrint, <OnFlag>) | Boolean value | Specifies whether to include layers set not to print |
| Include drawings paper color | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportIncludeDrawingsPaperColor)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPDFExportIncludeDrawingsPaperColor, <OnFlag>) | Boolean value |  |