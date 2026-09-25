<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDerivedPatternFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IDerivedPatternFeatureData Interface |

The following tables list the members exposed by [IDerivedPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [DrivingFeatureSkippedItemArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~DrivingFeatureSkippedItemArray.html) | Gets the skipped instances in the driving feature of this derived pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [ForceUseSeedConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~ForceUseSeedConfiguration.html) | Gets or sets whether to synchronize the configuration of pattern components with the configuration of the seed component in this derived pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PatternFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~PatternFeature.html) | Gets or sets the pattern feature for this derived pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PropagateVisualProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~PropagateVisualProperty.html) | Gets or sets whether to propagate visual properties (e.g., colors, textures, etc.) in this derived pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [SeedComponentArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~SeedComponentArray.html) | Gets or sets an array of seed component features for this derived pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [SeedPosition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~SeedPosition.html) | Gets or sets which pattern instance to use as the seed feature for this derived pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [SkippedItemArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~SkippedItemArray.html) | Gets or sets the list of skipped items for this derived pattern feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~AccessSelections.html) | Gains access to the selections that describe this derived pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSeedComponentCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~GetSeedComponentCount.html) | Gets the number of seed component features for this derived pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSkippedItemCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~GetSkippedItemCount.html) | Gets the number of skipped items for this derived pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~GetTransform.html) | Gets the transform for the specified instance of this derived-pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~IAccessSelections.html) | Obsolete. See [IDerivedPatternFeatureData::IAccessSelections2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDerivedPatternFeatureData~IAccessSelections2.html). |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~IAccessSelections2.html) | Gains access to the selections that describe this derived pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetSeedComponentArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~IGetSeedComponentArray.html) | Gets the seed component features for this derived pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetSkippedItemArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~IGetSkippedItemArray.html) | Gets the list of skipped items for this derived pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetSeedComponentArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~ISetSeedComponentArray.html) | Sets an array of the seed component features for this derived pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetSkippedItemArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~ISetSkippedItemArray.html) | Sets the list of items to skip for this derived pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections that describe this derived pattern feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IDerivedPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)