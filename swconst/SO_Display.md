<!-- source: swconst/SO_Display.htm -->

# SOLIDWORKS API Help

# System Options > Display

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture of the
  dialog corresponds to the settings
  on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on
  the dialog but are now obsolete.

![](SO_Display.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Hidden edges displayed as - Solid | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesHiddenEdgeDisplay)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesHiddenEdgeDisplay, swEdgesHiddenEdgeDisplay\_e.swEdgesHiddenEdgeDisplaySolid) | swEdgesHiddenEdgeDisplay\_e.swEdgesHiddenEdgeDisplaySolid |  |
| Hidden edges displayed as - Dashed | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesHiddenEdgeDisplay)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesHiddenEdgeDisplay, swEdgesHiddenEdgeDisplay\_e.swEdgesHiddenEdgeDisplayDashed) | swEdgesHiddenEdgeDisplay\_e.swEdgesHiddenEdgeDisplayDashed |  |
| Part/Assembly tangent edge display - As visible | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesTangentEdgeDisplay)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesTangentEdgeDisplay, swEdgesTangentEdgeDisplay\_e.swEdgesTangentEdgeDisplayVisible) | swEdgesTangentEdgeDisplay\_e.swEdgesTangentEdgeDisplayVisible |  |
| Part/Assembly tangent edge display - As phantom | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesTangentEdgeDisplay)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesTangentEdgeDisplay, swEdgesTangentEdgeDisplay\_e.swEdgesTangentEdgeDisplayPhantom) | swEdgesTangentEdgeDisplay\_e.swEdgesTangentEdgeDisplayPhantom |  |
| Part/Assembly tangent edge display - Removed | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesTangentEdgeDisplay)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesTangentEdgeDisplay, swEdgesTangentEdgeDisplay\_e.swEdgesTangentEdgeDisplayRemoved) | swEdgesTangentEdgeDisplay\_e.swEdgesTangentEdgeDisplayRemoved |  |
| Edge display in shaded with edges mode - HLR | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesShadedModeDisplay)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesShadedModeDisplay, swEdgesShadedModeDisplay\_e.swEdgesShadedModeDisplayHLR) | swEdgesShadedModeDisplay\_e.swEdgesShadedModeDisplayHLR |  |
| Edge display in shaded with edges mode - HLR - Optimize for thin parts | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesShadedModeDisplayOptimizeForThinParts)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesShadedModeDisplayOptimizeForThinParts, <OnFlag>) | Boolean value | True to optimize for thin parts; valid only if **Edge display in shaded with edges mode - HLR** is set |
| Edge display in shaded with edges mode - Wireframe | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesShadedModeDisplay)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesShadedModeDisplay, swEdgesShadedModeDisplay\_e.swEdgesShadedModeDisplayWireframe) | swEdgesShadedModeDisplay\_e.swEdgesShadedModeDisplayWireframe) |  |
| Assembly transparency for in context edit - <selection box> | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesInContextEditTransparencyType)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesInContextEditTransparencyType, swInContextEditTransparencyType\_e.<Value>) | See swInContextEditTransparencyType\_e for valid options |  |
| Assembly transparency for in context edit - <slider> | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesInContextEditTransparency)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swEdgesInContextEditTransparency, <Value>) | Integer value between 0 and 100 indicating transparency |  |
| Anti-aliasing | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemOptionDisplayAntiAliasing)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemOptionDisplayAntiAliasing, <Value>) | See swSystemOptionDisplayAntiAliasing\_e for valid options |

S pecifies whether to smooth out jagged edges in Shaded With Edges, Wireframe, Hidden Lines Removed, and Hidden Lines Visible modes |

| Use shaded face highlighting | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseShadedFaceHighlight)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseShadedFaceHighlight, <OnFlag>) | Boolean value |  |
| Highlight all edges of features selected in graphics view | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesHighlightFeatureEdges)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesHighlightFeatureEdges, <OnFlag>) | Boolean value | Specifies whether all edges on selected feature are highlighted when feature selected |
| Dynamic highlight from graphics view | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesDynamicHighlight)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesDynamicHighlight, <OnFlag>) | Boolean value | Specifies whether to highlight edges, faces, vertices, dimensions, annotations, and so on, in the graphics area when pointer moves across them |
| Display temporary axes upon hover over cylindrical faces | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayTempAxesOnMouseHover)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayTempAxesOnMouseHover, <OnFlag>) | Boolean value |  |
| Show open edges of surfaces in different color | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesOpenEdgesDifferentColor)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesOpenEdgesDifferentColor, <OnFlag>) | Boolean value | Specifies whether to differentiate between open edges of surface and any tangent edges or silhouette |
| Display shaded planes | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesDisplayShadedPlanes)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesDisplayShadedPlanes, <OnFlag>) | Boolean value | Specifies whether to display transparent shaded planes with a wireframe edge that have different front and back colors |
| Display dimensions flat to screen | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayDimensionsFlatToScreen)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayDimensionsFlatToScreen, <OnFlag>) | Boolean value | Specifies whether to display dimensions flat to screen |
| Display notes flat to screen | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayNotesFlatToScreen)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayNotesFlatToScreen, <OnFlag>) | Boolean value | Specifies whether to display notes flat to screen |
| Display reference triad | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayReferenceTriad)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayReferenceTriad, <OnFlag>) | Boolean value |  |
| Display scrollbars in graphics view for parts and assemblies | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayScrollbarsInGraphicsViewPartsAndAssemblies)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayScrollbarsInGraphicsViewPartsAndAssemblies, <OnFlag>) | Boolean value |  |
| Display scrollbars in graphics view for drawings | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayScrollbarsInGraphicsViewDrawings)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayScrollbarsInGraphicsViewDrawings, <OnFlag>) | Boolean value |  |
| Display draft quality ambient occlusion | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDraftQualityAmbientOcclusion)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDraftQualityAmbientOcclusion, <OnFlag>) | Boolean value | Specifies whether to use global lighting that adds realism to models by controlling the attenuation of ambient light due to occluded areas; available in all scenes when you use RealView graphics |
| Display Speedpak graphics circle | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplaySpeedpakGraphicsCircle)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplaySpeedpakGraphicsCircle, <OnFlag>) | Boolean value | Specifies whether to display Speedpak graphics circle |
| Display pattern information tooltips | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayPatternInformationToolTips)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayPatternInformationToolTips, <OnFlag>) | Boolean value | Specifies whether to display pattern information tooltips |
| Breadcrumbs - Show breadcrumbs on selection | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowBreadcrumbsOnSelection)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowBreadcrumbsOnSelection, <OnFlag>) | Boolean value | Specifies whether to show breadcrumbs on selection |
| Breatcrumbs - Show breadcrumbs at mouse pointer | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowBreadcrumbsAtMousePointer)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowBreadcrumbsAtMousePointer, <OnFlag>) | Boolean value | Specifies whether to show breadcrumbs at the mouse pointer; valid only if **Show breadcrumbs on selection** is selected |

Obsolete Enumerators

| Enumerator | Comment |
| swDisplayEquationIds | Obsolete |
| swFourViewportProjectionType | Obsolete |
| swDisplayGraphicsComponents | Obsolete |
| swDisplayReferenceGeometryForXYZOrientation | Obsolete |
| swEdgesAntiAlias | Obsolete |
| swEdgesHighQualityDisplay | Obsolete |
| swEdgesRepaintAfterSelectionInHLR | Obsolete |