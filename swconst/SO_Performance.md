<!-- source: swconst/SO_Performance.htm -->

# SOLIDWORKS API Help

# System Options - Performance

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture
  of the dialog corresponds to the settings
  on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on
  the dialog but are now obsolete.

![](SO_Performance.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Verification on rebuild | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceVerifyOnRebuild)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceVerifyOnRebuild, <OnFlag>) | Boolean value | Controls the level of error checking when you create or modify features. For most applications, the default setting (cleared) is adequate and results in a faster rebuild of the model |
| Ignores self-intersection check for some sheet metal features | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceSheetMetalIgnoreSelfIntersect)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceSheetMetalIgnoreSelfIntersect, <OnFlag>) | Boolean value | Specifies whether to suppress warning messages for certain sheet metal parts; for example, when flanges share a common edge and the part flattens correctly but displays a warning message |
| Transparency - High quality for normal view mode | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseAlphaTransparency)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseAlphaTransparency, <OnFlag>) | Boolean value | Specifies whether to change transparency quality from high to low when part or assembly is moving |
| Transparency - High quality for dynamic view mode | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swTransparencyHighQualityDynamic)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swTransparencyHighQualityDynamic, <OnFlag>) | Boolean value | Specifies whether high-quality transparency is retained while moving or rotating model with pan or rotate tools |
| Curvature generation | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceAlwaysGenerateCurvature)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceAlwaysGenerateCurvature, <OnFlag>) | Boolean value:   * True = Always (for every shaded model) * False = Only on demand | Specifies whether to always display curvature for shaded models |
| Level of detail | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLevelOfDetail)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swLevelOfDetail, <Value>) | Integer value ranging from 0 to 20 | Target frame rates ranging from 0 (off) to 20 (maximum level of detail removed); for example, if set at 20, then try and get 20FPS on spin dynamics by dropping detail until rate is achieved |
| Assembly loading - Automatically load component data on demand - or - Manually manage resolved and lightweight modes | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAssemblyLoadComponents)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swAssemblyLoadComponents, swAssemblyLoadComponents\_e.<Value>) | See swAssemblyLoadComponents\_e for options |  |
| Assembly loading - Load component lightweight | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceAssemblyLoadComponentsLightweight)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceAssemblyLoadComponentsLightweight, <OnFlag>) | Boolean value | Valid only if Assembly loading - Manually manage resolved and lightweight modes is selected |
| Assembly loading - Always resolve subassemblies | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceAlwaysResolveSubassemblies)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPerformanceAlwaysResolveSubassemblies, <OnFlag>) | Boolean value | Specifies whether to always resolve subassemblies when an assembly opens lightweight; Valid only if Assembly loading - Manually manage resolved and lightweight modes is selected |
| Assembly loading - Check out-of-date lightweight components | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCheckForOutOfDateLightweightComponents)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCheckForOutOfDateLightweightComponents, swCheckOutOfDate\_e.<Value>) | See swCheckOutOfDate\_e for valid options | Valid only if Assembly loading - Manually manage resolved and lightweight modes is selected |
| Assembly loading - Resolve lightweight components | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swResolveLightweight)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swResolveLightweight, swPromptAlwaysNever\_e.<Value>) | Boolean value:   * 0 = Prompt * 1 = Always | Valid only if Assembly loading - Manually manage resolved and lightweight modes is selected |
| Assembly loading - Rebuild assembly on load: | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPerformanceAssemRebuildOnLoad)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swPerformanceAssemRebuildOnLoad, swPromptAlwaysNever\_e.<Value>) | See swPromptAlwaysNever\_e for valid options | Valid only if Assembly loading - Manually manage resolved and lightweight modes is selected |
| Mates - Mate animation speed | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swMateAnimationSpeed)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swMateAnimationSpeed, <Value>) | Double value:   * 0 = off * >0 = animation speed in seconds | Specifies speed of animation for mates |
| Mates - SmartMate Sensitivity | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSmartMateSensitivity)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSmartMateSensitivity, <Value>) | Double value:   * 0 = off * >0 = animation speed in seconds | Specifies the speed at which SmartMates are applied |
| Mates - Magnetic mate pre-alignment | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swMagMatePreAlign)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swMagMatePreAlign, <OnFlag>) | Boolean value | Specifies whether to enable magnetic mates pre-alignment |
| Save - Purge cached configuration data | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPurgeAllBodiesForNonActiveConfigurations)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPurgeAllBodiesForNonActiveConfigurations, <OnFlag>) | Boolean value | Specifies whether to purge cached configuration data to reduce file size and save time |
| Save - Update mass properties while saving document | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUpdateMassPropsDuringSave)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUpdateMassPropsDuringSave, <OnFlag>) | Boolean value | Specifies whether to update mass properties information when saving document |
| Use shaded preview | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseShadedPreview)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseShadedPreview, <OnFlag>) | Boolean value | Specifies whether to use shaded preview |
| Use software OpenGL | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swUseSimpleOpenGL) | Read-only Boolean value | Specifies whether graphics adapter hardware acceleration is disabled and graphics rendering using only software is enabled |
| Enhanced graphics performance (requires SOLIDWORKS restart) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnablePerformancePipeline)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnablePerformancePipeline, <OnFlag>) | Boolean value |  |

Obsolete Enumerators

| Enumerator | Comment |
| swPerformanceRemoveDetailDuringZoomPanRotate | Obsolete; specified whether to remove small components and faces (both interior and exterior) from graphics area when zooming, panning, or rotating model to improve system performance |
| swPerformanceSave | Obsolete |
| swPerformancePreviewDuringOpen | Obsolete; specified whether to preview the model while opening it |