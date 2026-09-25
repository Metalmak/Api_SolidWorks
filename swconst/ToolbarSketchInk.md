<!-- source: swconst/ToolbarSketchInk.htm -->

# SOLIDWORKS API Help

# Sketch Ink Toolbar

Visible only on Windows 10:

![](ToolbarSketchInk.gif)

| Setting | Get/Set Methods | Return Value or <Value> or <OnFlag> | **Comments** |
| Pen > Colors | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPenSketchStrokeColor)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPenSketchStrokeColor, <Value>) | COLORREF value | COLORREF values in SOLIDWORKS  IColorTable; use function RGB to convert R,G, and B values to COLORREF values; the following colors are displayed in the graphic from left to right and top to bottom: RGB(0,0,0) RGB(102,102,102) RGB(153,153,153) RGB(221,221,221) RGB(255,255,255) RGB(204,0,0) RGB(255,153,0) RGB(255,255,0) RGB(0,158,15) RGB(153,0,255) RGB(255,0,255) RGB(147,196,125) RGB(255,217,102) RGB(142,124,195) RGB(194,123,160) RGB(111,168,220) RGB(56,118,29) RGB(224,102,102) RGB(97,61,48) |
| Pen > Size | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPenSketchStrokeThickness)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPenSketchStrokeThickness, <Value>) | Valid options as defined in swLineWeights\_e:  swLW\_THIN  swLW\_NORMAL  swLW\_THICK  swLW\_THICK2  swLW\_THICK3  swLW\_THICK4  swLW\_THICK5 | Thickness of pen stroke; if you set an invalid value (<0 or >6) then the pen size is automatically set to swLW\_THIN = 0 |