<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IBoundaryBossFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IBoundaryBossFeatureData Interface |

The following tables list the members exposed by [IBoundaryBossFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AutoSelect](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~AutoSelect.html) | Gets or sets whether to automatically select all or only specific bodies for the boundary feature to affect in the multibody part. |
| ![ Property](dotnetimages/Property.gif) | [D1CurveInfluence](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~D1CurveInfluence.html) | Gets or sets the type of curve influence for Direction 1 for this boundary feature. |
| ![ Property](dotnetimages/Property.gif) | [D1Curves](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~D1Curves.html) | Gets or sets the curves for Direction 1 for this boundary feature. |
| ![ Property](dotnetimages/Property.gif) | [D2CurveInfluence](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~D2CurveInfluence.html) | Gets or sets the type of curve influence for Direction 2 for this boundary feature. |
| ![ Property](dotnetimages/Property.gif) | [D2Curves](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~D2Curves.html) | Gets or sets the curves for Direction 2 for this boundary feature. |
| ![ Property](dotnetimages/Property.gif) | [FeatureScope](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~FeatureScope.html) | Gets or sets whether to use scope for the boundary feature in a multibody part. |
| ![ Property](dotnetimages/Property.gif) | [FeatureScopeBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~FeatureScopeBodies.html) | Gets or sets the bodies that this boundary feature affects in a multibody part. |
| ![ Property](dotnetimages/Property.gif) | [FeatureScopeBodiesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~FeatureScopeBodiesCount.html) | Gets the number of bodies that this boundary feature affects in a multibody part. |
| ![ Property](dotnetimages/Property.gif) | [MergeResult](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~MergeResult.html) | Gets or sets whether to merge all boundary feature elements. |
| ![ Property](dotnetimages/Property.gif) | [MergeTangentFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~MergeTangentFaces.html) | Gets or sets whether to make the surfaces in the resulting boundary feature tangent if the corresponding boundary segments are tangent. |
| ![ Property](dotnetimages/Property.gif) | [ThinFeatureReversed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~ThinFeatureReversed.html) | Gets whether this thin feature boundary feature is reversed. |
| ![ Property](dotnetimages/Property.gif) | [ThinFeatureThickness](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~ThinFeatureThickness.html) | Gets or sets the thickness of this thin feature boundary feature. |
| ![ Property](dotnetimages/Property.gif) | [ThinFeatureType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~ThinFeatureType.html) | Gets or sets the type of thin feature for this boundary feature. |
| ![ Property](dotnetimages/Property.gif) | [TrimByD1](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~TrimByD1.html) | Gets whether to trim surfaces in Direction 1 when curves do not form a closed boundary feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~AccessSelections.html) | Gains access to the selections that define this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetAlignmentType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetAlignmentType.html) | Gets the type of alignment for the specified curve in the specified direction for this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetCurvesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetCurvesCount.html) | Gets the number of curves in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetDirectionVector](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetDirectionVector.html) | Gets the entity used as the direction vector for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetDraftAngle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetDraftAngle.html) | Gets the draft angle for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetDraftAngleReverseDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetDraftAngleReverseDirection.html) | Gets whether the draft angle is flipped for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetGuideTangencyType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetGuideTangencyType.html) | Gets the type of tangency for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTangentApplyToAll](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetTangentApplyToAll.html) | Gets whether one handle that controls all constraints for the entire profile is displayed for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTangentDirectionReversed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetTangentDirectionReversed.html) | Gets whether the direction of adjacent tangent faces is flipped for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTangentInfluence](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetTangentInfluence.html) | Gets the curve influence for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTangentLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~GetTangentLength.html) | Gets the tangent length, which controls the amount of influence for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [IsThinFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~IsThinFeature.html) | Gets whether the boundary feature is a thin feature. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections for this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [SetAlignmentType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetAlignmentType.html) | Sets the type of alignment for the specified curve in the specified direction for this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [SetDirectionVector](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetDirectionVector.html) | Sets the entity to use as the direction vector for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [SetDraftAngle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetDraftAngle.html) | Sets the draft angle for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [SetDraftAngleReverseDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetDraftAngleReverseDirection.html) | Sets whether the draft angle is flipped for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [SetGuideTangencyType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetGuideTangencyType.html) | Sets the type of tangency for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [SetTangentApplyToAll](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetTangentApplyToAll.html) | Sets whether to display one handle that controls all constraints for the entire profile for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [SetTangentDirectionReversed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetTangentDirectionReversed.html) | Sets whether the direction of adjacent tangent faces is flipped for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [SetTangentInfluence](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetTangentInfluence.html) | Sets the curve influence toward the next curve for the specified curve in the specified direction in this boundary feature. |
| ![ Method](dotnetimages/Method.gif) | [SetTangentLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData~SetTangentLength.html) | Sets the tangent length, which controls the amount of influence for the specified curve in the specified direction in this boundary feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IBoundaryBossFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::InsertNetBlend Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertNetBlend.html)

[IFeatureManager::SetNetBlendCurveData Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetNetBlendCurveData.html)

[IFeatureManager::SetNetBlendDirectionData Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetNetBlendDirectionData.html)