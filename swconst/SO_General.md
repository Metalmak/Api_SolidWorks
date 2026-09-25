<!-- source: swconst/SO_General.htm -->

# SOLIDWORKS API Help

# System Options > General

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture corresponds to the settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on the dialog
  but are now obsolete.

![](SO_General.gif)

| Setting | Get/Set Methods | Return Value   or   <Value>   or   <OnFlag> | Comment |
| Recent documents - Maximum recent documents displayed | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swMaximumRecentDocuments)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swMaximumRecentDocuments, <Value>) | 1 <= Integer value <= 100 | Specifies how many documents to display in the **File > Open Recent** list |
| Recent documents - Include documents opened from other documents | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIncludeDocumentsOpenedFromOtherDocuments)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIncludeDocumentsOpenedFromOtherDocuments, <OnFlag>) | Boolean value | Specifies whether to include the documents opened from other documents in the **File > Open Recent** list |
| Recent documents - Open last used document(s) at startup | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swOpenLastUsedDocumentAtStart)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swOpenLastUsedDocumentAtStart, <OnFlag>) | Boolean value | Specifies whether to open the last-used document when starting up SOLIDWORKS software; true if always, false if never |
| Input dimension value | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swInputDimValOnCreate)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swInputDimValOnCreate, <OnFlag>) | Boolean value | Specifies whether to automatically display Modify dialog when dimensioning new entities |
| Single command per pick | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSingleCommandPerPick)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSingleCommandPerPick, <OnFlag>) | Boolean value | Specifies whether to deselect sketch and dimension tools after each use |
| Use shaded face highlighting | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseShadedFaceHighlight)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseShadedFaceHighlight, <OnFlag>) | Boolean value | Specifies whether selected faces are displayed in a solid color (green by default) |
| Show thumbnail graphics in File Explorer | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swThumbnailGraphics)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swThumbnailGraphics, <OnFlag>) | Boolean value | Specifies whether thumbnail graphic instead of an icon in File Explorer is displayed for each SOLIDWORKS part or assembly document |
| Use system separator for dimensions | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseSystemSeparatorForDims)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseSystemSeparatorForDims, <OnFlag>) | Boolean value | Specifies whether default system decimal separator is used when displaying decimal numbers |
| Use English language menus | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseEnglishLanguage)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseEnglishLanguage, <OnFlag>) | Boolean value | Specifies whether to change to English if another language was selected when SOLIDWORKS software was installed;  SOLIDWORKS software must be restarted for this change to take effect |
| Use English language feature and file names | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseEnglishLanguageFeatureNames)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseEnglishLanguageFeatureNames, <OnFlag>) | Boolean value | Specifies whether to use English feature and file names in languages other than English |
| Enable Confirmation Corner | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnableConfirmationCorner)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnableConfirmationCorner, <OnFlag>) | Boolean value | Specifies whether to display Confirmation Corner in the upper-right corner of the graphics area |
| Auto-show PropertyManager | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoShowPropertyManager)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoShowPropertyManager, <OnFlag>) | Boolean value | Specifies whether to automatically display PropertyManager when editing an entity |
| Auto-size PropertyManager when panels are split | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSizePropertyManager)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSizePropertyManager, <OnFlag>) | Boolean value | Specifies whether to autosize PropertyManager pages when panels are split |
| Automatically edit macro after recording | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEditMacroAfterRecord)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEditMacroAfterRecord, <OnFlag>) | Boolean value | Specifies whether to automatically edit a macro after recording it  NOTE: If after recording a macro you select to save the macro as all macro types (.swp, .csproj, and .vbproj), then this option has no effect. |
| Stop VSTA debugger on macro exit | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swStopDebuggingVstaOnExit)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swStopDebuggingVstaOnExit, <OnFlag>) | Boolean value | Specifies whether to stop the debugger when the macro exits main()  IMPORTANT: When debugging VSTA macros with user-interface components such as PropertyManager pages, manipulators, or other objects that use events or handler objects, it is necessary to keep the debugger running after the main() method of the VSTA macro exits. |
| Enable FeatureXpert | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUserEnableAutoFix)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUserEnableAutoFix, <OnFlag>) | Boolean value | Specifies whether to enable FeatureXpert |
| Enable Freeze bar | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUserEnableFreezeBar)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUserEnableFreezeBar, <OnFlag>) | Boolean value | Specifies whether to enable or disable the freeze bar |
| When rebuild error occurs | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swRebuildErrorAction)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swRebuildErrorAction, swStopContinuePrompt\_e.<Value>) | See swStopContinuePrompt\_e for valid options |  |
| Custom property used as component description | ISldWorks::GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swCustomPropertyUsedAsComponentDescription)  ISldWorks::SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swCustomPropertyUsedAsComponentDescription, <Value>) | String value |  |
| Show latest Technical Alerts and News in Welcome dialog (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowNewsFeedsInTaskPane)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowNewsFeedsInTaskPane, <OnFlag>) | Boolean value | Specifies whether to show the latest Technical Alerts and News in the Welcome dialog |
| Check for solutions when SOLIDWORKS crashes | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swCheckCrashSolutions)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swCheckCrashSolutions, <OnFlag>) | Boolean value |  |
| Enable sounds for SOLIDWORKS events | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnableSoundsForSOLIDWORKSEvents)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnableSoundsForSOLIDWORKSEvents, <OnFlag>) | Boolean value |  |
| Allow cosmetic threads for upgrade | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnableAllowCosmeticThreadsUpgrade)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnableAllowCosmeticThreadsUpgrade, <OnFlag>) | Boolean value | Specifies whether to upgrade cosmetic threads to the latest design |
| Create configuration tables on open | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swCreateConfigurationTableOnOpen) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swCreateConfigurationTableOnOpen, <OnFlag>) | Boolean value |  |
| **SOLIDWORKS Customer Experience Improvement Program** - Help make SOLIDWORKS products better by automatically sending your log files to DS SOLIDWORKS Corporation (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPerformanceFeedback)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPerformanceFeedback, swPerformanceFeedback\_e.<Value>) | See swPerformanceFeedback\_e for valid options | Specifies whether to enable or disable performance feedback or when to remind the user to enable it |

Obsolete Enumerators

| Enumerator | Comment |
| swEnablePerformanceEmail | Obsolete |
| swEnablePerformanceFeedback | Obsolete; use swUserPreferenceIntegerValue\_e.swPerformanceFeedback (shown in previous table) |
| swEnablePropertyManager | Obsolete; always enabled |
| swMaximizeDocumentOnOpen | Obsolete |
| swSaveEModelData | Obsolete |
| swShowDimensionNames | Obsolete |
| swEnableVSTAVersion3 | Obsolete |