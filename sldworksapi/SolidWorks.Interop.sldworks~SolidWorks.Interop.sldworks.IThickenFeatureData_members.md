<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IThickenFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IThickenFeatureData Interface |

The following tables list the members exposed by [IThickenFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AutoSelect](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~AutoSelect.html) | Gets or sets whether to automatically select all or only specific bodies for the thicken feature to affect in a multibody part. |
| ![ Property](dotnetimages/Property.gif) | [FeatureScope](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~FeatureScope.html) | Gets or sets whether to use scope for the thicken feature in a multibody part. |
| ![ Property](dotnetimages/Property.gif) | [FeatureScopeBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~FeatureScopeBodies.html) | Gets or sets the solid bodies that the thicken feature affects in a multibody part. |
| ![ Property](dotnetimages/Property.gif) | [FillVolume](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~FillVolume.html) | Gets or sets whether to fill a volume with this thicken feature. |
| ![ Property](dotnetimages/Property.gif) | [Merge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~Merge.html) | Gets or sets whether to merge the results of this thicken feature in a multibody part. |
| ![ Property](dotnetimages/Property.gif) | [Surface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~Surface.html) | Gets or sets the thickened surface. |
| ![ Property](dotnetimages/Property.gif) | [Thickness](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~Thickness.html) | Gets or sets the thickness for this thicken feature. |
| ![ Property](dotnetimages/Property.gif) | [ThicknessSide](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~ThicknessSide.html) | Gets or sets which side to apply thickness. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~AccessSelections.html) | Gains access to the selections that define this thicken feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFeatureScopeBodiesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~GetFeatureScopeBodiesCount.html) | Gets the number of solid bodies affected by the thicken feature in a multibody part. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~IAccessSelections.html) | Gains access to the selections that define this thicken feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetFeatureScopeBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~IGetFeatureScopeBodies.html) | Gets the solid bodies that the thicken feature affects in a multibody part. |
| ![ Method](dotnetimages/Method.gif) | [IsBossFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~IsBossFeature.html) | Gets whether this feature is a boss or a cut. |
| ![ Method](dotnetimages/Method.gif) | [ISetFeatureScopeBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~ISetFeatureScopeBodies.html) | Sets the solid bodies that the thicken feature affects in a multibody part. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData~ReleaseSelectionAccess.html) | Releases the selections that created this thicken feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IThickenFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::FeatureBossThicken Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureBossThicken.html)

[IFeatureManager::FeatureCutThicken Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureCutThicken.html)