<!-- source: swconst/FileSaveAsTIFPSDOptions.htm -->

# SOLIDWORKS API Help

# System Options > Export > TIF/PSD/JPG/PNG

To display the dialog:

Click **Tools > Options > System Options > Export > TIF/PSD/JPG/PNG** in
**File Format**.

- or -

1. Click **File > Save As**.
2. In **Save as type**, select **Tif**, **Adobe PhotoShop
   File**s, **JPEG**, or **Portable Network Graphics**.
3. Click **Options**.

![](FileSaveAsTIFPSDOptions.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Output as - Image type | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffImageType)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffImageType, swTiffImageType\_e.<Value>) | See swTiffImageType\_e for valid options |  |
| Output as - Tiff Compression scheme | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffCompressionScheme)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffCompressionScheme, swTiffCompressionScheme\_e.<Value>) | See swTiffCompressionScheme\_e for valid options |  |
| Output as - Remove background | See Comment | See Comment | Currently not available in the SOLIDWORKS API |
| Output as - Jpeg Compression | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportJpegCompression)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swExportJpegCompression, <Value>) | Long value (1-100) | 1 is for lowest compression; 100 is for highest compression (low quality) |
| Output as - Screen capture | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffScreenOrPrintCapture)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffScreenOrPrintCapture, <Value>) | 0 |  |
| Output as - Print capture | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffScreenOrPrintCapture)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffScreenOrPrintCapture, <Value>) | 1 |  |
| Output as - All sheets (multipage) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintAllSheets)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintAllSheets, <OnFlag>) | True | For Output as - Print capture only |
| Output as - Current sheet | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintAllSheets)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintAllSheets, <OnFlag>) | False | For Output as - Print capture only |
| Output as - Use sheet size(s) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintUseSheetSize)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintUseSheetSize, <OnFlag>) | True | For Output as - Print capture only |
| Output as - Use print size | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintUseSheetSize)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintUseSheetSize, <OnFlag>) | False | For Output as - Print capture only |
| Output as - Enable text padding (for low DPI/size settings) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintPadText)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintPadText, <OnFlag>) | Boolean value | Adjusts inter-character text spacing such that the text fills the bounding rectangle of the string; set to True when using low DPI and small paper sizes (A, A4, or A3) |
| Output as - Include layers set not to print | SldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTIFIncludeLayersNotToPrint)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTIFIncludeLayersNotToPrint, <OnFlag>) | Boolean value | Specifies whether to include layers set not to print |
| Output as - Include drawings paper color | SldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTIFExportIncludeDrawingsPaperColor)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTIFExportIncludeDrawingsPaperColor, <OnFlag>) | Boolean value |  |
| Print capture options - DPI | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffPrintDPI)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffPrintDPI, <Value>) | Integer value | For drawings only; For Output as - Print capture only |
| Print capture options - Paper size | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffPrintPaperSize)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffPrintPaperSize, swDwgPaperSizes\_e.<Value>) | See swDwgPaperSizes\_e for valid options |  |
| Print capture options - Width | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swTiffPrintDrawingPaperWidth)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swTiffPrintDrawingPaperWidth, <Value>) | Double value in meters | For drawings only; For Output as - Print capture only with Print capture options - Paper size set to User Defined |
| Print capture options - Height | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swTiffPrintDrawingPaperHeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swTiffPrintDrawingPaperHeight, <Value>) | Double value in meters | For drawings only; For Output as - Print capture only with Print capture options - Paper size set to User Defined |
| Print capture options - Scale to fit | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintScaleToFit)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTiffPrintScaleToFit, <OnFlag>) | Boolean value | For drawings only; specifies whether to scale drawing to fit page |
| Print capture options - Scale | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffPrintScaleFactor)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTiffPrintScaleFactor, <Value>) | Integer value | Specifies the scale factor |