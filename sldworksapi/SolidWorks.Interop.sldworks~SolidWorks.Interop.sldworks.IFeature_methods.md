<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_methods.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IFeature Interface Methods | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IFeature Interface |

For a list of all members of this type, see [IFeature members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html).

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddComment](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~AddComment.html) | Adds a comment to this feature. |
| ![ Method](dotnetimages/Method.gif) | [AddPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~AddPropertyExtension.html) | Adds a property extension to this feature. |
| ![ Method](dotnetimages/Method.gif) | [BreakLink](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~BreakLink.html) | Breaks the link to third-party native CAD parts and assemblies. |
| ![ Method](dotnetimages/Method.gif) | [DeSelect](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~DeSelect.html) | Deselects this feature. |
| ![ Method](dotnetimages/Method.gif) | [EnumDisplayDimensions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~EnumDisplayDimensions.html) | This method returns a [display dimensions enumeration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEnumDisplayDimensions.html) for this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetAffectedFaceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetAffectedFaceCount.html) | Gets the number of faces modified by a feature, such as a draft feature. |
| ![ Method](dotnetimages/Method.gif) | [GetAffectedFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetAffectedFaces.html) | Gets the faces modified by a feature, such as a draft feature. |
| ![ Method](dotnetimages/Method.gif) | [GetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetBody.html) | Obsolete. Superseded by [IFeatures::GetFaces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetFaces.html), [IFeatures::IGetFaces2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IGetFaces2.html), [IFace2::GetBody](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetBody.html), and [IFace2::IGetBody](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IGetBody.html). |
| ![ Method](dotnetimages/Method.gif) | [GetBox](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetBox.html) | Gets the bounding box for this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetChildren](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetChildren.html) | Gets the child features belonging to this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetCreatedVersion](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetCreatedVersion.html) | Gets the SOLIDWORKS version number in which the selected feature was created. |
| ![ Method](dotnetimages/Method.gif) | [GetDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDefinition.html) | Gets the feature data object for a feature, such as an advanced mate, extrusion, loft, fillet, chamfer, etc., in order to access the parameters that control the definition of this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetDisplayDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDisplayDimension.html) | Gets the display dimension object for the specified pattern property. |
| ![ Method](dotnetimages/Method.gif) | [GetEditStatus](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetEditStatus.html) | Gets whether the feature can currently be edited. |
| ![ Method](dotnetimages/Method.gif) | [GetErrorCode](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetErrorCode.html) | Obsolete. Superseded by [IFeature::GetErrorCode2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetErrorCode2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetErrorCode2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetErrorCode2.html) | Gets the error code for this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFaceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetFaceCount.html) | Gets the number of faces in this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetFaces.html) | Gets the faces in this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFirstDisplayDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetFirstDisplayDimension.html) | Provides access to the dimensions that belong to this feature by returning the first display dimension associated with this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFirstSubFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetFirstSubFeature.html) | Gets the first sub-feature that belongs to this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetID.html) | Gets the feature ID of this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetImportedFeatureParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetImportedFeatureParameters.html) | Gets the data object for this 3D Interconnect part or assembly. |
| ![ Method](dotnetimages/Method.gif) | [GetImportedFileName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetImportedFileName.html) | Gets the file name from an imported feature. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialIdName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetMaterialIdName.html) | Gets the material name. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetMaterialPropertyValues.html) | Obsolete. Superseded by [IFeature::GetMaterialPropertyValues2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetMaterialPropertyValues2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetMaterialPropertyValues2.html) | Gets the material property values for this feature in the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialUserName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetMaterialUserName.html) | Gets the material name for this feature, which is visible to the user. |
| ![ Method](dotnetimages/Method.gif) | [GetModifiedVersion](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetModifiedVersion.html) | Gets the SOLIDWORKS version number in which this feature was last modified. |
| ![ Method](dotnetimages/Method.gif) | [GetNameForSelection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetNameForSelection.html) | Gets the selected feature's type and name. |
| ![ Method](dotnetimages/Method.gif) | [GetNextDisplayDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetNextDisplayDimension.html) | Gets the next display dimension associated with this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetNextFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetNextFeature.html) | Gets the next feature in the part. |
| ![ Method](dotnetimages/Method.gif) | [GetNextSubFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetNextSubFeature.html) | Gets the next sub-feature from the owner of this sub-feature. |
| ![ Method](dotnetimages/Method.gif) | [GetOwnerFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetOwnerFeature.html) | Gets the feature that owns this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetParents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetParents.html) | Gets the parent features for this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetPropertyExtension.html) | Gets the property extension on this feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSpecificFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetSpecificFeature.html) | Obsolete. Superseded by [IFeature::GetSpecificFeature2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetSpecificFeature2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSpecificFeature2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetSpecificFeature2.html) | Gets the more specific interface to a selected feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetTexture.html) | Gets the texture applied to this feature in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetTypeName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetTypeName.html) | Gets the type of feature.  **NOTE:** To get the underlying type of feature of an Instant3D feature (i.e., "ICE"), call this method; otherwise, call [IFeature::GetTypeName2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetTypeName2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetTypeName2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetTypeName2.html) | Gets the type of feature.  **NOTE:** To get the underlying type of feature of an Instant3D feature (i.e., "ICE"), call [IFeature::GetTypeName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetTypeName.html); otherwise, call this method. |
| ![ Method](dotnetimages/Method.gif) | [GetUIState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetUIState.html) | Gets the user-interface state of the current feature. |
| ![ Method](dotnetimages/Method.gif) | [GetUpdateStamp](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetUpdateStamp.html) | Gets the current update stamp for this feature. |
| ![ Method](dotnetimages/Method.gif) | [HasFrozenUpdatePending](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~HasFrozenUpdatePending.html) | Gets whether this feature has pending freeze updates. |
| ![ Method](dotnetimages/Method.gif) | [HasMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~HasMaterialPropertyValues.html) | Gets whether this feature has an appearance. |
| ![ Method](dotnetimages/Method.gif) | [IGetAffectedFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetAffectedFaces.html) | Gets the faces modified by a feature, such as a draft feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetBody.html) | Obsolete. Superseded by [IFeatures::GetFaces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetFaces.html), [IFeatures::IGetFaces2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IGetFaces2.html), [IFace2::GetBody](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetBody.html), and [IFace2::IGetBody](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IGetBody.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetBody2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetBody2.html) | Obsolete. Superseded by [IFeatures::GetFaces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetFaces.html), [IFeatures::IGetFaces2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IGetFaces2.html), [IFace2::GetBody](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetBody.html), and [IFace2::IGetBody](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IGetBody.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetBox](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetBox.html) | Gets the bounding box for this feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetChildCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetChildCount.html) | Gets the number of child features that belong to this feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetChildren](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetChildren.html) | Gets the child features belonging to this feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetDefinition.html) | Gets the feature data object for a feature, such as an extrusion, loft, fillet, chamfer, etc., in order to access the parameters that control the definition of this feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetFaces.html) | Obsolete. Superseded by [IFeature::IGetFaces2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IGetFaces2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetFaces2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetFaces2.html) | Gets the faces in this feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetFirstSubFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetFirstSubFeature.html) | Gets the first sub-feature that belongs to this feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetMaterialPropertyValues.html) | Obsolete. Superseded by [IFeature::IGetMaterialPropertyValues2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IGetMaterialPropertyValues2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetMaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetMaterialPropertyValues2.html) | Gets the material property values for this feature in the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [IGetNextFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetNextFeature.html) | Gets the next feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetNextSubFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetNextSubFeature.html) | Gets the next sub-feature from the owner of this sub-feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetParentCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetParentCount.html) | Gets the number of parent features for this feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetParents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetParents.html) | Gets the parent features for this feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetSpecificFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetSpecificFeature.html) | Obsolete. Superseded by [IFeature::GetSpecificFeature2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetSpecificFeature2.html). |
| ![ Method](dotnetimages/Method.gif) | [IIsSuppressed2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IIsSuppressed2.html) | Gets whether the feature in the specified configurations is suppressed. |
| ![ Method](dotnetimages/Method.gif) | [IListExternalFileReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IListExternalFileReferences.html) | Obsolete. Superseded by [IFeature::IListExternalFileReferences2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IListExternalFileReferences2.html). |
| ![ Method](dotnetimages/Method.gif) | [IListExternalFileReferences2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IListExternalFileReferences2.html) | Gets the names and statuses of the external references for this feature in a part or assembly. |
| ![ Method](dotnetimages/Method.gif) | [IModifyDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IModifyDefinition.html) | Obsolete. Superseded by [IFeature::IModifyDefinition2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IModifyDefinition2.html). |
| ![ Method](dotnetimages/Method.gif) | [IModifyDefinition2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IModifyDefinition2.html) | Updates the definition of a feature with the new values in an associated feature data object obtained with [IFeature::IGetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IGetDefinition.html). |
| ![ Method](dotnetimages/Method.gif) | [IParameter](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IParameter.html) | Gets a pointer to the object for the specified parameter or a pointer to the specified parameter. |
| ![ Method](dotnetimages/Method.gif) | [IRemoveMaterialProperty2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IRemoveMaterialProperty2.html) | Removes material property values from this feature. |
| ![ Method](dotnetimages/Method.gif) | [IsBase](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsBase.html) | Obsolete. Superseded by [IFeature::IsBase2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IsBase2.html). |
| ![ Method](dotnetimages/Method.gif) | [IsBase2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsBase2.html) | Gets whether this feature is a base feature. |
| ![ Method](dotnetimages/Method.gif) | [IsDimXpertAnnotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsDimXpertAnnotation.html) | Gets whether this feature is a DimXpert annotation. |
| ![ Method](dotnetimages/Method.gif) | [IsDimXpertFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsDimXpertFeature.html) | Gets whether this feature is a DimXpert feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ISetBody.html) | Obsolete. Superseded by [IFeature::ISetBody3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~ISetBody3.html). |
| ![ Method](dotnetimages/Method.gif) | [ISetBody2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ISetBody2.html) | Obsolete. Superseded by [IFeature::ISetBody3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~ISetBody3.html). |
| ![ Method](dotnetimages/Method.gif) | [ISetBody3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ISetBody3.html) | Replaces the body of the base feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ISetMaterialPropertyValues.html) | Obsolete. Superseded by [IFeature::ISetMaterialPropertyValues2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~ISetMaterialPropertyValues2.html). |
| ![ Method](dotnetimages/Method.gif) | [ISetMaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ISetMaterialPropertyValues2.html) | Sets the material property values for this feature in the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [ISetSuppression2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ISetSuppression2.html) | Sets the suppression state of this feature. |
| ![ Method](dotnetimages/Method.gif) | [IsFrozen](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsFrozen.html) | Gets whether this feature is frozen. |
| ![ Method](dotnetimages/Method.gif) | [IsHiddenLock](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsHiddenLock.html) | Gets whether this feature is the freeze bar. |
| ![ Method](dotnetimages/Method.gif) | [IsRolledBack](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsRolledBack.html) | Gets whether this feature is rolled back. |
| ![ Method](dotnetimages/Method.gif) | [IsSuppressed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsSuppressed.html) | Obsolete. Superseded by [IFeature::IsSuppressed2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IsSuppressed2.html). |
| ![ Method](dotnetimages/Method.gif) | [IsSuppressed2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsSuppressed2.html) | Gets whether the feature in the specified configurations is suppressed. |
| ![ Method](dotnetimages/Method.gif) | [ListExternalFileReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ListExternalFileReferences.html) | Obsolete. Superseded by [IFeature::ListExternalFileReferences2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~ListExternalFileReferences2.html). |
| ![ Method](dotnetimages/Method.gif) | [ListExternalFileReferences2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ListExternalFileReferences2.html) | Gets the names and statuses of the external references on the feature in a part or assembly. |
| ![ Method](dotnetimages/Method.gif) | [ListExternalFileReferencesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ListExternalFileReferencesCount.html) | Gets the number of external references on the feature in a part or assembly. |
| ![ Method](dotnetimages/Method.gif) | [MakeSubFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~MakeSubFeature.html) | Makes a feature become a subfeature of this feature. |
| ![ Method](dotnetimages/Method.gif) | [ModifyDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ModifyDefinition.html) | Updates the definition of a feature with the new values in an associated feature data object obtained with [IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html). |
| ![ Method](dotnetimages/Method.gif) | [MoveFreezeBarTo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~MoveFreezeBarTo.html) | Obsolete. Superseded by [IFeature::MoveFreezeBarTo2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~MoveFreezeBarTo2.html). |
| ![ Method](dotnetimages/Method.gif) | [MoveFreezeBarTo2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~MoveFreezeBarTo2.html) | Moves the freeze bar to the specified location in the FeatureManager design tree. |
| ![ Method](dotnetimages/Method.gif) | [Parameter](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~Parameter.html) | Gets a pointer to the object for the specified parameter or a pointer to the specified parameter. |
| ![ Method](dotnetimages/Method.gif) | [RemoveMaterialProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~RemoveMaterialProperty.html) | Obsolete. Superseded by [IFeature::RemoveMaterialProperty2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~RemoveMaterialProperty2.html). |
| ![ Method](dotnetimages/Method.gif) | [RemoveMaterialProperty2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~RemoveMaterialProperty2.html) | Removes material property values from this feature. |
| ![ Method](dotnetimages/Method.gif) | [RemoveTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~RemoveTexture.html) | Removes texture from this feature in either all of the configurations or only the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [RemoveTextureByDisplayState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~RemoveTextureByDisplayState.html) | Removes texture from this feature in the specified display state. |
| ![ Method](dotnetimages/Method.gif) | [ResetPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ResetPropertyExtension.html) | Deletes the property extension for this feature. |
| ![ Method](dotnetimages/Method.gif) | [Select](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~Select.html) | Obsolete. Superseded by [IFeature::Select2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~Select2.html). |
| ![ Method](dotnetimages/Method.gif) | [Select2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~Select2.html) | Selects and marks this feature. |
| ![ Method](dotnetimages/Method.gif) | [SelectByMark](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SelectByMark.html) | Obsolete. Superseded by [IFeature::Select2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~Select2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetBodiesToKeep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetBodiesToKeep.html) | Set the bodies to keep and their configurations for features that create multiple bodies in parts and assemblies. |
| ![ Method](dotnetimages/Method.gif) | [SetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetBody.html) | Obsolete. Superseded by [IFeature::SetBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~SetBody2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetBody2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetBody2.html) | Replaces an imported base feature body. |
| ![ Method](dotnetimages/Method.gif) | [SetImportedFeatureParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetImportedFeatureParameters.html) | Sets the data object for this 3D Interconnect part or assembly. |
| ![ Method](dotnetimages/Method.gif) | [SetImportedFileName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetImportedFileName.html) | Sets the file name of an imported feature. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialIdName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetMaterialIdName.html) | Sets the material name for this feature. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetMaterialPropertyValues.html) | Obsolete. Superseded by [IFeature::SetMaterialPropertyValues2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~SetMaterialPropertyValues2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetMaterialPropertyValues2.html) | Sets the material property values for this feature in the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialUserName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetMaterialUserName.html) | Sets the material user name for this feature, which is visible to the user. |
| ![ Method](dotnetimages/Method.gif) | [SetSuppression](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetSuppression.html) | Obsolete. Superseded by [IFeature::SetSuppression2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~SetSuppression2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetSuppression2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetSuppression2.html) | Sets the suppression state of this feature. |
| ![ Method](dotnetimages/Method.gif) | [SetTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetTexture.html) | Applies texture to this feature in either all configurations or only the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [SetTextureByDisplayState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetTextureByDisplayState.html) | Applies texture to this feature in the specified display state. |
| ![ Method](dotnetimages/Method.gif) | [SetUIState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetUIState.html) | Sets the user-interface state of the current feature. |
| ![ Method](dotnetimages/Method.gif) | [Update3DInterconnectModel](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~Update3DInterconnectModel.html) | Updates the model for this 3D Interconnect part or assembly. |
| ![ Method](dotnetimages/Method.gif) | [UpdateExternalFileReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~UpdateExternalFileReferences.html) | Updates the external file references on this model. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)