<!-- source: swconst/SO_Miscellaneous.htm -->

# SOLIDWORKS API Help

# System Options > Miscellaneous

Some system-level enumerators exist in the SOLIDWORKS API that do not
correspond to any of the options shown on the SOLIDWORKS Tools > Options
> System Options dialogs. Click the links to jump to the tables in this
topic containing these miscellaneous system-level enumerators.

NOTE: Unlinked text does not
have any miscellaneous system-level enumerators. Unlinked text is shown
to help you more easily map these miscellaneous system-level enumerators with the system
options shown on the Tools > Options
> System Options tab.

See System
Options and Document Properties for details about system options and
document properties.

| Miscellaneous System-level Enumerators | |
| Related to categories on System Options tab | Not related to categories on System Options tab |
| [General](#General)  [Drawings](#Drawings)    - Display Style    - Area Hatch/Fill    - Performance  [Colors](#Colors)  [Sketch](#Sketch)    - Relations/Snaps  [Display](#Display/Selection)  Selection  [Performance](#Performance)  [Assemblies](#Assemblies)  [External References](#ExternalReferences)  Default Templates  [File Locations](#FileLocations)  [FeatureManager](#FeatureManager)  Spin Box Increments  [View](#View)  Backup/Recover  Hole Wizard/Toolbox  [File Explorer](#FileExplorer)  Search  [Collaboration](#Collaboration)  Messages/Errors/Warnings Import Export | [Bill of Materials](#BillofMaterials)  [Detailing](#Detailing)  [Display States](#DisplayStates)  [Large Assembly Mode](#LargeAssemblyMode)  [PropertyManager](#PropertyManager)  [Quick Tips](#QuickTips)  [Reference Triad](#ReferenceTriad)  [Shaded Sketch Contours](#ShaddedSketchContours)  [Viewpoint](#Viewpoint) [My SOLIDWORKS](#MySolidworks) |

General

| Enumerator | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| swEditDesignTableInSeparateWindow | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEditDesignTableInSeparateWindow)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEditDesignTableInSeparateWindow, <OnFlag>) | Boolean value | Specifies whether to open Excel worksheet in Excel window or in SOLIDWORKS graphics view |
| swNotifySNLNotObtainedForEDrawingsSave | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swNotifySNLNotObtainedForEDrawingsSave)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swNotifySNLNotObtainedForEDrawingsSave, <OnFlag>) | Boolean value | Specifies whether to display message box each time eDrawings file saved |
| swUndoStepsMaximum | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swUndoStepsMaximum)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swUndoStepsMaximum, <Value>) | Integer value | Specifies the maximum number of Undo steps allowed; the higher the number, the more memory used |

[Back to top](#Top)

Drawings

| Enumerator | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| swAutomaticDrawingViewUpdateForceOff | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutomaticDrawingViewUpdateForceOff)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutomaticDrawingViewUpdateForceOff, <OnFlag>) | Boolean value | Specifies whether to automatically update drawing views |
| swDrawingAutomaticModelDimPlacement | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingAutomaticModelDimPlacement)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingAutomaticModelDimPlacement, <OnFlag>) | Boolean value | Specifies whether inserted dimensions are automatically placed at appropriate distance from geometry in view |
| swDrawingDefaultSheetScaleDenominator | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDrawingDefaultSheetScaleDenominator)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDrawingDefaultSheetScaleDenominator, <Value> ) | Double value | Specifies denominator for default drawing sheet scale |
| swDrawingDefaultSheetScaleNumerator | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDrawingDefaultSheetScaleNumerator)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDrawingDefaultSheetScaleNumerator, <Value>) | Double value | Specifies numerator for default drawing sheet scale |
| swDrawingDisplayViewBorders | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingDisplayViewBorders)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingDisplayViewBorders, <OnFlag>) | Boolean value | Specifies whether borders are displayed around individual drawing views |
| swDynamicDrawingViewActivation | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDynamicDrawingViewActivation)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDynamicDrawingViewActivation, <OnFlag>) | Boolean value | Specifies whether the view closest to pointer is automatically activated |
| swDrawingPrintCrosshatchOutOfDateViews | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawingPrintCrosshatchOutOfDateViews)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawingPrintCrosshatchOutOfDateViews, swPromptAlwaysNever\_e.<Value>) | See swPromptAlwaysNever\_e for valid options | Specifies what happens when a drawing with out-of-date views is printed or print-previewed |
| swDrawingViewSmoothDynamicMotion | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingViewSmoothDynamicMotion)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingViewSmoothDynamicMotion, <OnFlag>) | Boolean value | Specifies whether dynamic operations, such as panning and zooming, display smoothly |

[Back to top](#Top)

Colors

NOTE: The input or output value
is the corresponding IColorTable
value unless otherwise specified.

| Enumerator | Get/Set Methods | Return Value  or  <Value> | Comment |
| swSystemColorsActiveSelectionListBox | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsActiveSelectionListBox)  ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsActiveSelectionListBox, <Value>) | Integer value | RGB value |
| swSystemColorsCrossHair | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsCrossHair)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsCrossHair, <Value>) | Integer value | RGB value |
| swSystemColorsDrawingsLockedFocus | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsDrawingsLockedFocus)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsDrawingsLockedFocus, <Value>) | Integer value | Border color; RGB value |
| swSystemColorsDrawingsSheetBorder | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsDrawingsSheetBorder)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsDrawingsSheetBorder, <Value>) | Integer value | Drawing sheet border color;  RGB value |
| swSystemColorsDrawingsViewBorder | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsDrawingsViewBorder)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsDrawingsViewBorder, <Value>) | Integer value | View border color;  RGB value |
| swSystemColorsNoteEditHandle | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsNoteEditHandle)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsNoteEditHandle, <Value>) | Integer value | RGB value |
| swSystemColorsNoteHandle | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsNoteHandle)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsNoteHandle, <Value>) | Integer value | RGB value |
| swSystemColorsTemporarySketchDragging | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsTemporarySketchDragging)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsTemporarySketchDragging, <Value>) | Integer value | RGB value |
| swSystemColorsTreeViewBackground | ISldWorks::GetUserPreferenceIntegerValue (swUserPreferenceIntegerValue\_e.swSystemColorsTreeViewBackground) | Integer value | Read-only RGB value |
| swSystemColorsWeldPathSelection | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsWeldPathSelection)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSystemColorsWeldPathSelection, <Value>) | Integer value | RGB value |

[Back to top](#Top)

Sketch

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| Display virtual sharps | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayVirtualSharps)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayVirtualSharps, <OnFlag>) | Boolean value | Specifies whether to create sketch point at the virtual intersection point of two sketch entities |

[Back to top](#Top)

Display

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swDisplayMissingRefsWhenEditFeature | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayMissingRefsWhenEditFeature)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayMissingRefsWhenEditFeature, <OnFlag>) | Boolean value | Specifies whether to display missing references when editing features |
| swEdgesShadedEdgesDifferentColor | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesShadedEdgesDifferentColor)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesShadedEdgesDifferentColor, <OnFlag>) | Boolean value | Specifies whether to apply specified color to model edges when model is in Shaded With Edges mode |

[Back to top](#Top)

Performance

| Enumerator | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| swPerformanceDynamicUpdateOnMove | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceDynamicUpdateOnMove)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceDynamicUpdateOnMove, <OnFlag>) | Boolean value | Specifies whether to display feature preview while dragging entities of sketch |
| swPerformanceWin95ZoomClipping | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceWin95ZoomClipping)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceWin95ZoomClipping, <OnFlag>) | Boolean value | Valid for Windows ME only; specifies whether selected portion of model can be zoomed in on |
| swPerformanceViewsToDraftQuality | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPerformanceViewsToDraftQuality)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPerformanceViewsToDraftQuality, <Value>) | * 0 = Prompt * 1 = Always * 2 = Never | Specifies whether to automatically convert drawing views to draft quality when unloading components |
| swRebuildOnActivation | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swRebuildOnActivation)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swRebuildOnActivation, swRebuildOnActivation\_e.<Value>) | See swRebuildOnActivation\_e for valid options. |  |

[Back to top](#Top)

Assemblies

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swClearanceShowIgnored | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceShowIgnored)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceShowIgnored, <OnFlag>) | Boolean value | Specifies whether to show ignored clearances |
| swClearanceIgnoreEqual | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceIgnoreEqual)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceIgnoreEqual, <OnFlag>) | Boolean value | Specifies whether to ignore clearance equal to specified value |
| swClearanceSubAssyAsComp | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceSubAssyAsComp)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceSubAssyAsComp, <OnFlag>) | Boolean value | Specifies whether to treat subassemblies as components |
| swClearanceFasteners | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceFasteners)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceFasteners, <OnFlag>) | Boolean value | Specifies whether to create fasteners folder |
| swClearanceDisplayOption | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceDisplayOption)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swClearanceDisplayOption, <OnFlag>) | Boolean value | Specifies whether to make parts under study transparent |
| swIncontextFeatureHolderVisibility | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIncontextFeatureHolderVisibility)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIncontextFeatureHolderVisibility, <OnFlag>) | Boolean value | Specifies whether to hide or show all of the in-context icons |

[Back to top](#Top)

External References

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swWarnSavingReferencedDoc | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swWarnSavingReferencedDoc)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swWarnSavingReferencedDoc, <OnFlag>) | Boolean value | Specifies whether to display a warning when saving an assembly that references models that have been modified |

[Back to top](#Top)

File Locations

| Enumerator | Get/Set Methods | Return Value  or  <Value> | Comment |
| swFileLocationsRouteCableLibrary | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swFileLocationsRouteCableLibrary)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swFileLocationsRouteCableLibrary, <Value>) | String value |  |
| swFileLocationsRouteComponentLibary | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swFileLocationsRouteComponentLibary)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swFileLocationsRouteComponentLibary, <Value>) | String value |  |
| swFileLocationsRouteCoveringLibrary | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swFileLocationsRouteCoveringLibrary)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swFileLocationsRouteCoveringLibrary, <Value>) | String value |  |

[Back to top](#Top)

FeatureManager

| Enumerator | Get/Set Methods | Return Value  or  <Value> | Comment |
| swFeatureManagerConfigTableFolderVisibility | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swFeatureManagerConfigTableFolderVisibility)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swFeatureManagerConfigTableFolderVisibility, swAutoHideShowResponse\_e.<Value>) | See swAutoHideShowResponse\_e for valid options |  |
| swFeatureManagerLightVisibility | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swFeatureManagerLightVisibility)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swFeatureManagerLightFolderVisibility, swAutoHideShowResponse\_e.<Value>) | See swAutoHideShowResponse\_e for valid options |  |

[Back to top](#Top)

View

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swInsertViewForNewDrawing | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swInsertViewForNewDrawing)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swInsertViewForNewDrawing, <OnFlag>) | Boolean value | Controls whether the Model View PropertyManager is automatically displayed when the user opens a new drawing |
| swViewShowAnnotationLinkErrors | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewShowAnnotationLinkErrors)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewShowAnnotationLinkErrors, <OnFlag>) | Boolean value | Specifies whether to show annotation link errors |
| swViewShowAnnotationLinkVariables | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewShowAnnotationLinkVariables)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewShowAnnotationLinkVariables, <OnFlag>) | Boolean value | Specifies whether to show annotation link variables |

[Back to top](#Top)

File Explorer

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |

|  |  |  |  |
| --- | --- | --- | --- |
|

swLockRecentDocumentsList |

ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLockRecentDocumentsList)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLockRecentDocumentsList, <OnFlag>) |

Boolean value | Specifies whether to lock the recent documents list to prevent opened documents from being added to it |

[Back to top](#Top)

Collaboration

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swCollabTopDocsNoPromptOrSave | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swCollabTopDocsNoPromptOrSave)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swCollabTopDocsNoPromptOrSave, <OnFlag>) | Boolean value | Specifies to not prompt to save read-only referenced documents |

[Back to top](#Top)

Bill of Materials

| Enumerator | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| swBomConfigurationAlignBottom | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swBomConfigurationAlignBottom)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swBomConfigurationAlignBottom, <OnFlag>) | Boolean value | For Excel-based BOMs only; specifies whether to add new items to BOM by extending top border of table |
| swBOMConfigurationAnchorType | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBOMConfigurationAnchorType)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBOMConfigurationAnchorType, swBOMConfigurationAnchorType\_e.<Value>) | See swBOMConfigurationAnchorType\_e for valid options |  |
| swBomConfigurationUseDocumentFont | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swBomConfigurationUseDocumentFont)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swBomConfigurationUseDocumentFont, <OnFlag>) | Boolean value | For Excel-based BOMs only; specifies whether to use document's note font when creating BOM |
| swBomConfigurationUseSummaryInfo | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swBomConfigurationUseSummaryInfo)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swBomConfigurationUseSummaryInfo, <OnFlag>) | Boolean value | For Excel-based BOMs only; specifies whether to use part identifier number in the title box of the Summary Info for the part number in the bill of materials |
| swBOMConfigurationWhatToShow | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBOMConfigurationWhatToShow)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBOMConfigurationWhatToShow, swBOMConfigurationWhatToShow\_e.<Value>) | See See swBOMConfigurationWhatToShow\_e for valid options for valid options |  |
| swBOMContentsDisplayAtTop | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swBOMContentsDisplayAtTop)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swBOMContentsDisplayAtTop, <OnFlag>) | Boolean value | For Excel-based BOMs only; specifies whether to show column headers at top of table |
| swBOMControlIDFromAssembly | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swBOMControlIDFromAssembly)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swBOMControlIDFromAssembly, <OnFlag>) | Boolean value | For Excel-based BOMs only; specifies whether row numbers follow assembly ordering |
| swBOMControlMissingRowDisplay | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBOMControlMissingRowDisplay)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBOMControlMissingRowDisplay, swBOMControlMissingRowDisplay\_e.<Value>) | See swBOMControlMissingRowDisplay\_e for valid options |  |
| swBOMControlMissingRows | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swBOMControlMissingRows)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swBOMControlMissingRows, <OnFlag>) | Boolean value | For Excel-based BOMs only; specifies whether rows for removed components are deleted from the table or displayed |
| swBOMControlSplitDirection | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBOMControlSplitDirection)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swBOMControlSplitDirection, swBOMControlSplitDirection\_e.<Value>) | See swBOMControlSplitDirection\_e for valid options |  |
| swBOMControlSplitHeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swBOMControlSplitHeight)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swBOMControlSplitHeight, <Value>) | Double value | Specifies BOM table height before splitting it; applies to Excel-based BOM tables only |
| swBOMControlSplitTable | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swBOMControlMissingRows)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swBOMControlMissingRows, <OnFlag>) | Boolean value | For Excel-based BOMs only; specifies whether BOM table can be split as indicated by swUserPreferenceIntegerValue\_e.swBOMControlSplitDirection and swUserPreferenceDoubleValue\_e.swBOMControlSplitHeight |

[Back to top](#Top)

Detailing

| Enumerator | Get/Set Methods | Return Value  or  <Value> | Comment |
| swDetailingDimFontHeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swDetailingDimFontHeight) | Double value in meters | Read-only; specifies height of dimensions |
| swDetailingNoteFontHeight | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.wDetailingNoteFontHeight) | Double value in meters | Read-only; specifies height of notes |

[Back to top](#Top)

Display States

| Enumerator | Get/Set Methods | Return Value  or  <Value> | Comment |
| swDisplayStateCreationChoice | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDisplayStateCreationChoice)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDisplayStateCreationChoice, swDisplayStateCreationChoices\_e.<Value>) | See swDisplayStateCreationChoices\_e for valid options | Specifies which display states to preserve for documents that:   * have both SOLIDWORKS colors and PhotoWorks material   display states * were saved in SOLIDWORKS   2009 or earlier |

[Back to top](#Top)

Large Assembly
Mode

| Enumerator | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| swLargeAsmModeAlwaysGenerateCurvature | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeAlwaysGenerateCurvature)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeAlwaysGenerateCurvature, <OnFlag>) | Boolean value | Specifies whether to always display curvatures for all shaded models |
| swLargeAsmModeAntiAliasEdgesFastMode | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeAntiAliasEdgesFastMode)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeAntiAliasEdgesFastMode, <OnFlag>) | Boolean value | Specifies whether to set HLR edges in shaded and fast HLR/HLV modes to anti-alias |
| swLargeAsmModeAutoActvate | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLargeAsmModeAutoActvate)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLargeAsmModeAutoActvate, <Value>) | * 0 = Prompt * 1 = Always * 2 = Never | In SOLIDWORKS 2006 and later, Prompt = Always |
| swLargeAsmModeAutoHideCompsDrawViewCreation | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeAutoHideCompsDrawViewCreation)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeAutoHideCompsDrawViewCreation, <Value>) | Boolean value | Specifies whether to automatically hide components on view creation |
| swLargeAsmModeAutoRecoverCount | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLargeAsmModeAutoRecoverCount)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLargeAsmModeAutoRecoverCount, <Value>) | Integer value |  |
| swLargeAsmModeCheckOutOfDateLightweight | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLargeAsmModeCheckOutOfDateLightweight)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLargeAsmModeCheckOutOfDateLightweight, <Value>) | * 0 = Do not check * 1 = Indicate * 2 = Always resolve |  |
| swLargeAsmModeDisplayModeForNewDrawViews | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLargeAsmModeDisplayModeForNewDrawViews)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLargeAsmModeDisplayModeForNewDrawViews, <Value>) | * 0 = Wireframe * 1 = Hidden Lines Visible * 2 = Hidden Lines Removed * 3 = Shaded | To set new drawing views to shaded with edges when in large assembly mode, set this enumerator to Shaded and set ISldWorks::SetUserPreferenceToggle  swUserPreferenceToggle\_e.swLargeAsmModeDrawingHLREdgesWhenShaded to true. |
| swLargeAsmModeDrawingAutoLoadModels | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeDrawingAutoLoadModels)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeDrawingAutoLoadModels, <Value>) | Boolean value | Specifies whether to automatically load models for detached drawings |
| swLargeAsmModeDrawingHLREdgesWhenShaded | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeDrawingHLREdgesWhenShaded)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeDrawingHLREdgesWhenShaded, <Value>) | Boolean value | Specifies whether default display style is shaded with edges.  NOTE: To set new drawing views to shaded with edges when in large assembly mode, set this enumerator to true and set ISldWorks::SetUserPreferenceIntegerValue swUserPreferenceIntegerValue\_e.swLargeAsmModeDisplayModeForNewDrawViews to shaded. |
| swLargeAsmModeDynHighlightFeatureMgr | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeDynHighlightFeatureMgr)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeDynHighlightFeatureMgr, <Value>) | Boolean value | Specifies whether entities in graphics area are highlighted when moving pointer over them in FeatureManager design tree |
| swLargeAsmModeDynHighlightGraphicsView | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeDynHighlightGraphicsView)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeDynHighlightGraphicsView, <Value>) | Boolean value | Specifies whether entities in the graphics area are highlighted when pointer is over them in graphics area |
| swLargeAsmModePreviewInsertComponents | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModePreviewInsertComponents)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModePreviewInsertComponents, <Value>) | Boolean value | Specifies whether to preview the assembly when inserting new components |
| swLargeAsmModeRemoveDetail | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeRemoveDetail)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeRemoveDetail, <Value>) | Boolean value | Specifies whether to remove details during zoom operations |
| swLargeAsmModeShadowsShadedMode | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeShadowsShadedMode)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeShadowsShadedMode, <Value>) | Boolean value | Specifies whether to show shadows in shaded mode |
| swLargeAsmModeShowContentsDragDrawView | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeShowContentsDragDrawView)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeShowContentsDragDrawView, <Value>) | Boolean value | Specifies whether to show contents or view boundary while dragging drawing view |
| swLargeAsmModeSmoothDynamicMotionDrawView | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeSmoothDynamicMotionDrawView)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeSmoothDynamicMotionDrawView, <Value>) | Boolean value | Specifies whether to smoothly pan and zoom dynamic operations in drawing views |
| swLargeAsmModeTransparencyDynamicViewMode | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeTransparencyDynamicViewMode)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeTransparencyDynamicViewMode, <Value>) | Boolean value | Specifies whether to use high quality transparency for dynamic view mode |
| swLargeAsmModeTransparencyNormalViewMode | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeTransparencyNormalViewMode)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeTransparencyNormalViewMode, <Value>) | Boolean value | Specifies whether to use high quality transparency for normal view mode |
| swLargeAsmModeUpdateMassPropsOnSave | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeUpdateMassPropsOnSave)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swLargeAsmModeUpdateMassPropsOnSave, <Value>) | Boolean value | Specifies whether to update mass properties when saving large assembly document |

[Back to top](#Top)

PropertyManager

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swPropertyManagerColorActiveClosedDivider | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorActiveClosedDivider) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorBackground | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorBackground) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColor\_Divider | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColor\_Divider) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorEditBox | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorEditBox) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColor\_EditText | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColor\_EditText) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorImportantMessage | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorImportantMessage) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorInnerBorder | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorInnerBorder) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorLabelAndIcon | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorLabelAndIcon) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorTitle | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorTitle) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorOuterBorder | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorOuterBorder) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorTopBorder | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorTopBorder) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorDivider | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyManagerColorDivider) | Read-only integer value for RGB color in use |  |
| swPropertyMgrDockingState | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceInteger\_e.swPropertyMgrDockingState) | See swPMContainer\_e for valid options |  |

[Back to top](#Top)

Quick Tips

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swQuickTipsAssembly | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickTipsAssembly)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickTipsAssembly, <OnFlag>) | Boolean value | Specifies whether to enable or disable Quick Tips in assembly documents |
| swQuickTipsDrawing | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickTipsDrawing)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickTipsDrawing, <OnFlag>) | Boolean value | Specifies whether to enable or disable Quick Tips in drawing documents |
| swQuickTipsPart | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickTipsPart)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swQuickTipsPart, <OnFlag>) | Boolean value | Specifies whether to enable or disable Quick Tips in part documents |

[Back to top](#Top)

Reference Triad

| Enumerator | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| swReferenceTriadUseAlternateLabel | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swReferenceTriadUseAlternateLabel)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swReferenceTriadUseAlternateLabel, <OnFlag>) | Boolean value | Indicates whether alternate text should replace the reference triad's standard text of X, Y, and Z; whenever you change this value, you must redraw the window to see the new text; use ISldWorks::SetUserPreferenceStringValue  swUserPreferenceStringValue\_e.swReferenceTriadXlabel, swUserPreferenceStringValue\_e.swReferenceTriadYLabel, and swUserPreferenceStringValue\_e.swReferenceTriadZLabel to specify the alternate text |
| swReferenceTriadXLabel | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swReferenceTriadXLabel)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swReferenceTriadXLabel, <Value>) | String value | Alternate text for the reference triad's standard text of X |
| swReferenceTriadYLabel | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swReferenceTriadYLabel)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swReferenceTriadYLabel, <Value>) | String value | Alternate text for the reference triad's standard text of Y |
| swReferenceTriadZLabel | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swReferenceTriadZLabel)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swReferenceTriadZLabel, <Value>) | String value | Alternate text for the reference triad's standard text of Z |

NOTE: Use ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swReferenceTriadUseAlternateLabels,
<OnFlag> to indicate whether
alternate text should replace the reference triad's standard text of X, Y,
or Z. If swUserPreferenceToggle\_e.swReferenceTriadUseAlernateLabels
is true and swReferenceTriadXLabel, swReferenceTriadYLabel, or swReferenceTriadZLabel
is blank, then the corresponding default text of X,
Y, or Z
is displayed.

[Back to top](#Top)

Shaded Sketch Contours

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swShadedSketchContours | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swShadedSketchContours)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swShadedSketchContours, <OnFlag>) | Boolean value | True to shade closed sketch contour areas, false to not |

[Back to top](#Top)

Viewpoint

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swViewpointPreserveNormals | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewpointPreserveNormals)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewpointPreserveNormals, <OnFlag>) | Boolean value | Specifies whether to preserve normals when saving document as Viewpoint file |

[Back to top](#Top)

My SolidWorks

| Enumerator | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| swMySldSettings | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swMySldSettings)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swMySldSettings, <Value>) | String value |  |

[Back to top](#Top)