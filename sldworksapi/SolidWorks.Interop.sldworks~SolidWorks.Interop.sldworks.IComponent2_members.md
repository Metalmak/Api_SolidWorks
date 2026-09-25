<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IComponent2 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IComponent2 Interface |

The following tables list the members exposed by [IComponent2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [ComponentReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ComponentReference.html) | Gets or sets a component reference for this component. |
| ![ Property](dotnetimages/Property.gif) | [DisplayTitle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~DisplayTitle.html) | Gets this component's title as displayed in the FeatureManager design tree. |
| ![ Property](dotnetimages/Property.gif) | [ExcludeFromBOM](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ExcludeFromBOM.html) | Obsolete. Superseded by [IComponent2::GetExcludeFromBOM2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetExcludeFromBOM2.html) and [IComponent2::SetExcludeFromBOM2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetExcludeFromBOM2.html). |
| ![ Property](dotnetimages/Property.gif) | [IMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IMaterialPropertyValues.html) | Gets or sets the material properties for the selected component in the active configuration. |
| ![ Property](dotnetimages/Property.gif) | [IsGraphicsOnly](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsGraphicsOnly.html) | Gets whether this component is graphics only. |
| ![ Property](dotnetimages/Property.gif) | [IsSpeedPak](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsSpeedPak.html) | Gets whether the active configuration for this component is SpeedPak. |
| ![ Property](dotnetimages/Property.gif) | [IsVirtual](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsVirtual.html) | Gets whether this component is a virtual component.  **NOTE:** **This property is a get-only property.** **Set is not implemented**. |
| ![ Property](dotnetimages/Property.gif) | [MaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~MaterialPropertyValues.html) | Gets or sets the material properties for the selected component in the active configuration. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Name.html) | Obsolete. Superseded by [IComponent2::Name2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Name2.html). |
| ![ Property](dotnetimages/Property.gif) | [Name2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Name2.html) | Gets or sets the name of the selected component. |
| ![ Property](dotnetimages/Property.gif) | [PresentationTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~PresentationTransform.html) | Gets or sets the component transform. |
| ![ Property](dotnetimages/Property.gif) | [ReferencedConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ReferencedConfiguration.html) | Gets or sets the active configuration used by this component. |
| ![ Property](dotnetimages/Property.gif) | [ReferencedDisplayState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ReferencedDisplayState.html) | Obsolete. Superseded by [IComponent2::ReferencedDisplayState2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ReferencedDisplayState2.html). |
| ![ Property](dotnetimages/Property.gif) | [ReferencedDisplayState2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ReferencedDisplayState2.html) | Gets or sets the active display state of this component. |
| ![ Property](dotnetimages/Property.gif) | [Solving](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Solving.html) | Gets the **Solve as** option (rigid or flexible) of this component. |
| ![ Property](dotnetimages/Property.gif) | [Transform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Transform.html) | Obsolete. Superseded by [IComponent2::Transform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Transform2.html). |
| ![ Property](dotnetimages/Property.gif) | [Transform2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Transform2.html) | Gets or sets the component transform. |
| ![ Property](dotnetimages/Property.gif) | [UseNamedConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~UseNamedConfiguration.html) | Gets whether a specified configuration or the in-use/last active configuration is used. |
| ![ Property](dotnetimages/Property.gif) | [Visible](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Visible.html) | Gets or sets the visibility state of this component. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~AddPropertyExtension.html) | Adds a property extension to this component. |
| ![ Method](dotnetimages/Method.gif) | [DeSelect](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~DeSelect.html) | Deselects this component. |
| ![ Method](dotnetimages/Method.gif) | [EnumBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~EnumBodies.html) | Obsolete. Superseded by [IComponent2::EnumBodies2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~EnumBodies2.html). |
| ![ Method](dotnetimages/Method.gif) | [EnumBodies2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~EnumBodies2.html) | Obsolete. Superseded by [IComponent2::EnumBodies3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~EnumBodies3.html). |
| ![ Method](dotnetimages/Method.gif) | [EnumBodies3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~EnumBodies3.html) | Gets the bodies in the component in a multibody part. |
| ![ Method](dotnetimages/Method.gif) | [EnumRelatedBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~EnumRelatedBodies.html) | Creates an enumerated list of bodies. |
| ![ Method](dotnetimages/Method.gif) | [EnumSectionedBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~EnumSectionedBodies.html) | Gets the sectioned bodies seen in the specified view and returns them in an enumerated list. |
| ![ Method](dotnetimages/Method.gif) | [FeatureByName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~FeatureByName.html) | Gets the specified feature for this component. |
| ![ Method](dotnetimages/Method.gif) | [FindAttribute](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~FindAttribute.html) | Finds an attribute on a component. |
| ![ Method](dotnetimages/Method.gif) | [FirstFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~FirstFeature.html) | Gets the first feature in this component. |
| ![ Method](dotnetimages/Method.gif) | [GetBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBodies.html) | Obsolete. Superseded by [IComponent2::GetBodies2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetBodies2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetBodies2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBodies2.html) | Obsolete. Superseded by [IComponent2::GetBodies3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetBodies3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetBodies3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBodies3.html) | Gets the bodies in this component. |
| ![ Method](dotnetimages/Method.gif) | [GetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBody.html) | Gets the body that belongs to this instance of this component. |
| ![ Method](dotnetimages/Method.gif) | [GetBox](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBox.html) | Gets the bounding box for component. |
| ![ Method](dotnetimages/Method.gif) | [GetChildren](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetChildren.html) | Gets all of the children components of this component. |
| ![ Method](dotnetimages/Method.gif) | [GetConstrainedStatus](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetConstrainedStatus.html) | Gets the constrained status of this component. |
| ![ Method](dotnetimages/Method.gif) | [GetCorresponding](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetCorresponding.html) | Gets the corresponding object in the context of the assembly for a specific instance of the component. |
| ![ Method](dotnetimages/Method.gif) | [GetCorrespondingEntity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetCorrespondingEntity.html) | Gets the entity that corresponds with the Dispatch pointer in the context of the component. |
| ![ Method](dotnetimages/Method.gif) | [GetDecals](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetDecals.html) | Gets the decals applied to this component. |
| ![ Method](dotnetimages/Method.gif) | [GetDecalsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetDecalsCount.html) | Gets the number of decals applied to this component. |
| ![ Method](dotnetimages/Method.gif) | [GetDrawingComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetDrawingComponent.html) | Gets the drawing component for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetExcludeFromBOM2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetExcludeFromBOM2.html) | Gets whether this component is excluded from the bills of materials (BOMs) in the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [GetHiddenUnloadedChildrenCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetHiddenUnloadedChildrenCount.html) | Gets the number of hidden children components of this component that were not loaded when an assembly was [opened selectively](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDocumentSpecification~Selective.html). |
| ![ Method](dotnetimages/Method.gif) | [GetID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetID.html) | Gets the component ID for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetImportedPath](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetImportedPath.html) | Gets the full path name of the model imported for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialIdName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetMaterialIdName.html) | Gets the material name for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetMaterialPropertyValues2.html) | Gets the material properties for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialUserName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetMaterialUserName.html) | Gets the user-visible name of the material for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetMates](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetMates.html) | Gets the mates for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetModelDoc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetModelDoc.html) | Obsolete. Superseded by [IComponent2::GetModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetModelDoc2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetModelDoc2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetModelDoc2.html) | Gets the model document for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetModelMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetModelMaterialPropertyValues.html) | Gets the material properties of this lightweight component in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetModelTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetModelTexture.html) | Gets the texture applied to this lightweight component in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetParent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetParent.html) | Gets the parent component. |
| ![ Method](dotnetimages/Method.gif) | [GetPathName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetPathName.html) | Gets the full path name for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetPropertyExtension.html) | Gets the property extension on this component. |
| ![ Method](dotnetimages/Method.gif) | [GetReferencedDisplayStates](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetReferencedDisplayStates.html) | Gets the display states of this component that are referenced by the specified assembly display state(s). |
| ![ Method](dotnetimages/Method.gif) | [GetRenderMaterials](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetRenderMaterials.html) | Obsolete. Superseded by [IComponent2::GetRenderMaterials2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetRenderMaterials2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetRenderMaterials2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetRenderMaterials2.html) | Gets the appearances applied to this component in the specified display states. |
| ![ Method](dotnetimages/Method.gif) | [GetRenderMaterialsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetRenderMaterialsCount.html) | Obsolete. Superseded by [IComponent2::GetRenderMaterialsCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetRenderMaterialsCount2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetRenderMaterialsCount2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetRenderMaterialsCount2.html) | Gets the number of appearances applied to this component in the specified display states. |
| ![ Method](dotnetimages/Method.gif) | [GetSectionedBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetSectionedBodies.html) | Gets the sectioned bodies in the specified section view. |
| ![ Method](dotnetimages/Method.gif) | [GetSelectByIDString](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetSelectByIDString.html) | Gets the name of the component for possible use with [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html), for selectively opening a document using [ISldWorks::OpenDoc7](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~OpenDoc7.html) and [IDocumentSpecification](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDocumentSpecification.html), etc. |
| ![ Method](dotnetimages/Method.gif) | [GetSmartComponentData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetSmartComponentData.html) | Gets the features, components, and feature references of a Smart Component. |
| ![ Method](dotnetimages/Method.gif) | [GetSpecificTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetSpecificTransform.html) | Get the collapsed or exploded transform of a component when the assembly is exploded. |
| ![ Method](dotnetimages/Method.gif) | [GetSuppression](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetSuppression.html) | Obsolete. Superseded by [IComponent2::GetSuppression2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetSuppression2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSuppression2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetSuppression2.html) | Gets the suppression state of this component. |
| ![ Method](dotnetimages/Method.gif) | [GetTessNorms](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetTessNorms.html) | Gets the normal vector for each of the triangles, which make up the shaded picture tessellation for the component. |
| ![ Method](dotnetimages/Method.gif) | [GetTessTriangles](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetTessTriangles.html) | Gets the triangles that make up the shaded picture tessellation for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetTessTriStripEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetTessTriStripEdges.html) | Gets the edge IDs for the triangle strips. |
| ![ Method](dotnetimages/Method.gif) | [GetTessTriStripNorms](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetTessTriStripNorms.html) | Gets the normal vector for each of the triangles, which make up the shaded picture tessellation for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetTessTriStrips](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetTessTriStrips.html) | Gets the vertices that make up the shaded picture tessellation for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetTexture.html) | Gets the texture applied to this component in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetTotalTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetTotalTransform.html) | Combines the original transform of this component with the presentation transform of this component. |
| ![ Method](dotnetimages/Method.gif) | [GetUnloadedComponentNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetUnloadedComponentNames.html) | Gets the component's unloaded children components' path names, referenced configuration names, reasons why they are unloaded, document types, and names. |
| ![ Method](dotnetimages/Method.gif) | [GetVisibility](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetVisibility.html) | Gets the visibility state for this component. |
| ![ Method](dotnetimages/Method.gif) | [GetVisibilityInAsmDisplayStates](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetVisibilityInAsmDisplayStates.html) | Gets the visibilities of this component in the specified assembly display state(s). |
| ![ Method](dotnetimages/Method.gif) | [GetXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetXform.html) | Obsolete. Superseded by [IComponent2::Transform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Transform2.html). |
| ![ Method](dotnetimages/Method.gif) | [HasMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~HasMaterialPropertyValues.html) | Gets whether this component has an appearance. |
| ![ Method](dotnetimages/Method.gif) | [HasUnloadedComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~HasUnloadedComponents.html) | Gets whether this component has hidden or suppressed unloaded children components. |
| ![ Method](dotnetimages/Method.gif) | [IFindAttribute](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IFindAttribute.html) | Finds an attribute on a component. |
| ![ Method](dotnetimages/Method.gif) | [IGetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetBody.html) | Gets the body that belongs to this instance of this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetBox](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetBox.html) | Gets the bounding box for component. |
| ![ Method](dotnetimages/Method.gif) | [IGetChildren](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetChildren.html) | Gets all of the children components of this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetChildrenCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetChildrenCount.html) | Gets the number of children components for this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetCorrespondingEntity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetCorrespondingEntity.html) | Gets the entity that corresponds with the Dispatch pointer in the context of the component. |
| ![ Method](dotnetimages/Method.gif) | [IGetDecals](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetDecals.html) | Gets the decals applied to this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetMaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetMaterialPropertyValues2.html) | Gets the material properties for this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetMaterialPropertyValuesForFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetMaterialPropertyValuesForFace.html) | Gets the color of the specified face. |
| ![ Method](dotnetimages/Method.gif) | [IGetModelDoc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetModelDoc.html) | Obsolete. Superseded by [IComponent2::GetModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetModelDoc2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetModelMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetModelMaterialPropertyValues.html) | Gets the material properties of this lightweight component in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [IGetRenderMaterials](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetRenderMaterials.html) | Obsolete. Superseded by [IComponent2::GetRenderMaterials2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetRenderMaterials2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetTemporaryBodyID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTemporaryBodyID.html) | Gets the current body tag ID, which is not a permanent ID. |
| ![ Method](dotnetimages/Method.gif) | [IGetTessNorms](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTessNorms.html) | Gets the normal vector for each of the triangles, which make up the shaded picture tessellation for the component. |
| ![ Method](dotnetimages/Method.gif) | [IGetTessTriangleCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTessTriangleCount.html) | Gets the number of triangles that make up the shaded picture tessellation for this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetTessTriangles](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTessTriangles.html) | Gets the triangles that make up the shaded picture tessellation for this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetTessTriStripEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTessTriStripEdges.html) | Gets the edge IDs for the triangle strips. |
| ![ Method](dotnetimages/Method.gif) | [IGetTessTriStripEdgeSize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTessTriStripEdgeSize.html) | Gets the number of tessellation triangle edges. |
| ![ Method](dotnetimages/Method.gif) | [IGetTessTriStripNorms](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTessTriStripNorms.html) | Gets the normal vector for each of the triangles, which make up the shaded picture tessellation for this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetTessTriStrips](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTessTriStrips.html) | Gets the vertices that make up the shaded picture tessellation for this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetTessTriStripSize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTessTriStripSize.html) | Gets the array size of floats required to contain the data returned when calling [IComponent2::IGetTessTriStrips](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetTessTriStrips.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetVisibility](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetVisibility.html) | Gets the visibility state for this component. |
| ![ Method](dotnetimages/Method.gif) | [IGetXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetXform.html) | Obsolete. Superseded by [IComponent2::Transform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Transform2.html). |
| ![ Method](dotnetimages/Method.gif) | [IListExternalFileReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IListExternalFileReferences.html) | Obsolete. Superseded by [IComponent2::IListExternalFileReferences2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~IListExternalFileReferences2.html). |
| ![ Method](dotnetimages/Method.gif) | [IListExternalFileReferences2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IListExternalFileReferences2.html) | Gets the names and statuses of the external references on the component. |
| ![ Method](dotnetimages/Method.gif) | [IRemoveMaterialProperty2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IRemoveMaterialProperty2.html) | Removes material property values from the component. |
| ![ Method](dotnetimages/Method.gif) | [IsDisplayDataOutOfDate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsDisplayDataOutOfDate.html) | Gets the status of the display data for this component. |
| ![ Method](dotnetimages/Method.gif) | [IsEnvelope](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsEnvelope.html) | Gets whether this component is an envelope. |
| ![ Method](dotnetimages/Method.gif) | [ISetMaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ISetMaterialPropertyValues2.html) | Sets the material properties for this component. |
| ![ Method](dotnetimages/Method.gif) | [ISetVisibility](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ISetVisibility.html) | Sets the visibility state for this component. |
| ![ Method](dotnetimages/Method.gif) | [ISetXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ISetXform.html) | Obsolete. Superseded by [IComponent2::Transform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Transform2.html). |
| ![ Method](dotnetimages/Method.gif) | [ISetXformAndSolve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ISetXformAndSolve.html) | Obsolete. Superseded by [IComponent2::SetTransformAndSolve2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~SetTransformAndSolve2.html). |
| ![ Method](dotnetimages/Method.gif) | [IsFixed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsFixed.html) | Gets whether the component is fixed or floating. |
| ![ Method](dotnetimages/Method.gif) | [IsHidden](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsHidden.html) | Gets whether this component is hidden or suppressed. |
| ![ Method](dotnetimages/Method.gif) | [IsLoaded](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsLoaded.html) | Gets whether a component is loaded. |
| ![ Method](dotnetimages/Method.gif) | [IsMirrored](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsMirrored.html) | Gets whether this component is mirrored. |
| ![ Method](dotnetimages/Method.gif) | [IsNameOverridden](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsNameOverridden.html) | Gets whether the name of this component is overridden. |
| ![ Method](dotnetimages/Method.gif) | [IsPatternInstance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsPatternInstance.html) | Gets whether the component is a member of a pattern instance. |
| ![ Method](dotnetimages/Method.gif) | [IsRoot](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsRoot.html) | Gets whether this component is the root component. |
| ![ Method](dotnetimages/Method.gif) | [IsSmartComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsSmartComponent.html) | Gets whether this component is a Smart Component. |
| ![ Method](dotnetimages/Method.gif) | [IsSuppressed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsSuppressed.html) | Gets whether this component is suppressed. |
| ![ Method](dotnetimages/Method.gif) | [ListExternalFileReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ListExternalFileReferences.html) | Obsolete. Superseded by [IComponent2::ListExternalFileReferences2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~ListExternalFileReferences2.html). |
| ![ Method](dotnetimages/Method.gif) | [ListExternalFileReferences2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ListExternalFileReferences2.html) | Gets the names and statuses of the external file references on the component. |
| ![ Method](dotnetimages/Method.gif) | [ListExternalFileReferencesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ListExternalFileReferencesCount.html) | Gets the number of external references on the component. |
| ![ Method](dotnetimages/Method.gif) | [MakeVirtual](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~MakeVirtual.html) | Obsolete. by Superseded by [IComponent2::MakeVirtual2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~MakeVirtual2.html). |
| ![ Method](dotnetimages/Method.gif) | [MakeVirtual2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~MakeVirtual2.html) | Makes this component and optionally its child components virtual by saving them in the current assembly. |
| ![ Method](dotnetimages/Method.gif) | [RemoveMaterialProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~RemoveMaterialProperty.html) | Obsolete. Superseded by [IComponent2::RemoveMaterialProperty2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~RemoveMaterialProperty2.html). |
| ![ Method](dotnetimages/Method.gif) | [RemoveMaterialProperty2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~RemoveMaterialProperty2.html) | Removes the appearance from the component. |
| ![ Method](dotnetimages/Method.gif) | [RemovePresentationTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~RemovePresentationTransform.html) | Removes the presentation transform from this component. |
| ![ Method](dotnetimages/Method.gif) | [RemoveTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~RemoveTexture.html) | Removes the texture from this component in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [RemoveTextureByDisplayState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~RemoveTextureByDisplayState.html) | Removes the texture applied to this component in the specified display state. |
| ![ Method](dotnetimages/Method.gif) | [ReplaceReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ReplaceReference.html) | Obsolete. Superseded by [AssemblyDoc::ReplaceComponents](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~ReplaceComponents.html). |
| ![ Method](dotnetimages/Method.gif) | [ResetPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ResetPropertyExtension.html) | Clears all of the values stored in the property extension. |
| ![ Method](dotnetimages/Method.gif) | [SaveVirtualComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SaveVirtualComponent.html) | Saves a virtual component to an external file. |
| ![ Method](dotnetimages/Method.gif) | [Select](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Select.html) | Obsolete. Superseded by [IComponent2::Select3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Select3.html). |
| ![ Method](dotnetimages/Method.gif) | [Select2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Select2.html) | Obsolete. Superseded by [IComponent2::Select3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Select3.html). |
| ![ Method](dotnetimages/Method.gif) | [Select3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Select3.html) | Obsolete. Superseded by [IComponent2::Select4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Select4.html). |
| ![ Method](dotnetimages/Method.gif) | [Select4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Select4.html) | Selects this component. |
| ![ Method](dotnetimages/Method.gif) | [SelectByMark](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SelectByMark.html) | Obsolete. Superseded by [IComponent2::Select3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Select3.html). |
| ![ Method](dotnetimages/Method.gif) | [SetCosmosWorksMaterial](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetCosmosWorksMaterial.html) | Assigns the material to use during analysis to this component. |
| ![ Method](dotnetimages/Method.gif) | [SetExcludeFromBOM2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetExcludeFromBOM2.html) | Sets whether to exclude this component from the bills of materials (BOMs) in the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialIdName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetMaterialIdName.html) | Sets the material name for this component. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetMaterialPropertyValues2.html) | Sets the material properties for this component. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialUserName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetMaterialUserName.html) | Sets the material user name for this component. |
| ![ Method](dotnetimages/Method.gif) | [SetReferencedDisplayStates](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetReferencedDisplayStates.html) | Sets the specified display state of this component to be referenced by the specified assembly display state(s). |
| ![ Method](dotnetimages/Method.gif) | [SetSmartComponentData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetSmartComponentData.html) | Sets the features, components, and feature references of a Smart Component. |
| ![ Method](dotnetimages/Method.gif) | [SetSuppression](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetSuppression.html) | Obsolete. Superseded by [IComponent2::SetSuppression2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~SetSuppression2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetSuppression2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetSuppression2.html) | Sets the suppression state of this component. |
| ![ Method](dotnetimages/Method.gif) | [SetTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetTexture.html) | Applies texture to this component in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [SetTextureByDisplayState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetTextureByDisplayState.html) | Sets the texture applied to this component in the specified display state. |
| ![ Method](dotnetimages/Method.gif) | [SetTransformAndSolve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetTransformAndSolve.html) | Obsolete. Superseded by [IComponent2::SetTransformAndSolve2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~SetTransformAndSolve2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetTransformAndSolve2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetTransformAndSolve2.html) | Obsolete. Superseded by [IComponent2::SetTransformAndSolve3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetTransformAndSolve3.html). |
| ![ Method](dotnetimages/Method.gif) | [SetTransformAndSolve3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetTransformAndSolve3.html) | Sets the transform and solves for the mates for this component. |
| ![ Method](dotnetimages/Method.gif) | [SetVisibility](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetVisibility.html) | Sets the visibility state for this component. |
| ![ Method](dotnetimages/Method.gif) | [SetVisibilityInAsmDisplayStates](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetVisibilityInAsmDisplayStates.html) | Sets the visibility of this component in the specified assembly display state(s). |
| ![ Method](dotnetimages/Method.gif) | [SetXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetXform.html) | Obsolete. Superseded by [IComponent2::Transform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Transform2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetXformAndSolve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetXformAndSolve.html) | Obsolete. Superseded by [IComponent2::SetTransformAndSolve2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~SetTransformAndSolve2.html). |
| ![ Method](dotnetimages/Method.gif) | [UpdateExternalFileReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~UpdateExternalFileReferences.html) | Updates the external file references of this model. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IModelDoc2::GetPathName Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetPathName.html)