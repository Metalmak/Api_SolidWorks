<!-- source: swconst/SO_Drawings-DisplayStyle.htm -->

# SOLIDWORKS API Help

# System Options > Drawings > Display Style

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture
  of the dialog corresponds to the settings on
  that dialog.
* titled
  [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on the dialog
  but are now obsolete.

![](SO_Drawings-DisplayStyle.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or   <OnFlag> | Comment |
| Display style - Wireframe | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swHiddenEdgeDisplayDefault)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swHiddenEdgeDisplayDefault, <swDisplayMode\_e.swWIREFRAME) | See swDisplayMode\_e for valid options |  |
| Display style - Hidden lines visible | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swHiddenEdgeDisplayDefault)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swHiddenEdgeDisplayDefault, <swDisplayMode\_e.swHIDDEN\_GREYED) | See swDisplayMode\_e for valid options |  |
| Display style - Hidden lines removed | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swHiddenEdgeDisplayDefault)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swHiddenEdgeDisplayDefault, <swDisplayMode\_e.swHIDDEN) | See swDisplayMode\_e for valid options |  |
| Display style - Shaded with edges | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swHiddenEdgeDisplayDefault)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swHiddenEdgeDisplayDefault, <swDisplayMode\_e.swSHADED) | See swDisplayMode\_e for valid options | To display a drawing view shaded with edges, also set ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingsDefaultDisplayTypeHLREdgesWhenShaded, True) |
| Display style - Shaded | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingsDefaultDisplayTypeHLREdgesWhenShaded)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingsDefaultDisplayTypeHLREdgesWhenShaded, <OnFlag>) | Boolean value |  |
| Tangent edges - Visible | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTangentEdgeDisplayDefault)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTangentEdgeDisplayDefault, <swDisplayTangentEdges\_e.swTangentEdgesVisible) | See swDisplayTangentEdges\_e for valid options | Specifies tangent edges using a solid line |
| Tangent edges - Use font | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTangentEdgeDisplayDefault)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTangentEdgeDisplayDefault, <swDisplayTangentEdges\_e.swTangentEdgesVisibleAndFonted) | See swDisplayTangentEdges\_e for valid options | Specifies tangent edges using a line in the [default font](DP_LineFont.htm) |
| Tangent edges - Hide ends | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingHideEnds)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingHideEnds, <OnFlag>) | Boolean value | Specifies whether to hide the start and end segments of tangent edges |
| Tangent edges - Removed | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTangentEdgeDisplayDefault)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swTangentEdgeDisplayDefault, <swDisplayTangentEdges\_e.swTangentEdgesHidden) | See swDisplayTangentEdges\_e for valid options | Specifies to not display tangent edges |
| Edge quality for wireframe and hidden views - High/Draft  quality | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgeQualityWireframeHiddenViews)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgeQualityWireframeHiddenViews, False) | Boolean value | True for high edge quality for wireframe and hidden views; false for draft edge quality |
| Edge quality for shaded edge views - High/Draft quality | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgeQualityShadedEdgeViews)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgeQualityShadedEdgeViews, True) | Boolean value | True for high edge quality for shaded edge views; false for draft edge quality |

Obsolete Enumerators

| Enumerator | Comment |
| swDrawingsDefaultDisplayTypeFastHLRHLV | Obsolete; specified the display quality for new drawing views |