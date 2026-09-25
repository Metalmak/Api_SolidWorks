<!-- source: sldworksapi/ReleaseNotes-sldworksapi.html -->

![](images/collapse.gif)
![](images/expand.gif)
![](images/copycode.gif)
![](images/copycodeHighlight.gif)
![](images/drpdown.gif)
![](images/drpdown_orange.gif)

|  |
| --- |
|  |

|  |  |
| --- | --- |
| SOLIDWORKS API Help |  |
| Release Notes |
| Send Feedback | |

Glossary Item Box

This topic provides you with quick access to the enhancements in SOLIDWORKS API 2022.

##### Service Pack 3

#### IDocumentSpecification Interface

* [IDocumentSpecification::AddToRecentDocumentList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~AddToRecentDocumentList.html)

#### ISldWorks Interface

* [ISldWorks::GetBatchUploadedFilesInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetBatchUploadedFilesInfo.html)* [ISldWorks::GetFilePLMID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetFilePLMID.html)* [ISldWorks::RunBatchSaveProcess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RunBatchSaveProcess.html)* [ISldWorks::ShowBatchSaveTo3DExperienceDlg](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ShowBatchSaveTo3DExperienceDlg.html)

##### Service Pack 2

#### IComponent2 Interface

* [IComponent2::IsNameOverridden](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsNameOverridden.html)

#### IModelDocExtension Interface

* [IModelDocExtension::HasLegacyCThreads](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~HasLegacyCThreads.html)

#### ISldWorks Interface

* [ISldWorks::Get3DExperienceState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~Get3DExperienceState.html)

##### Service Pack 1

#### IFeatureManager Interface

* [IFeatureManager::ComponentPrimaryIdentifier](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~ComponentPrimaryIdentifier.html)* [IFeatureManager::ComponentSecondaryIdentifier](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~ComponentSecondaryIdentifier.html)* [IFeatureManager::ComponentTertiaryIdentifier](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~ComponentTertiaryIdentifier.html)* [IFeatureManager::HideComponentSingleConfigurationOrDisplayStateNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~HideComponentSingleConfigurationOrDisplayStateNames.html)* [IFeatureManager::SetComponentIdentifiers](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetComponentIdentifiers.html)

#### IModelDocExtension Interface

* [IModelDocExtension::Make3DExperienceCompatible](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~Make3DExperienceCompatible.html)

##### Service Pack 0

* [New functionality](#NewFunctionality0)* [New interfaces](#NewInterfaces0)* [New methods, properties, and delegates](#NewMethods0)* [Obsoleted methods and properties](#Obsoleted0)

###### New functionality

* Support for:

  + SOLIDWORKS Inspection.+ SOLIDWORKS PDM Professional Web API.+ Belt/chain assembly features. See [IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html), [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) and [IBeltChainFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData.html).+ Structure systems. See [IStructureSystemFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder.html), [IModelDocExtension::CreateStructureSystem](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateStructureSystem.html), [IModelDocExtension::CreateStructureSystemMemberData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateStructureSystemMemberData.html), [IFeatureManager::GetStructureSystemFolders](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~GetStructureSystemFolders.html), [IPrimaryMemberFacePlaneIntersectionFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData.html),
          [IPrimaryMemberPathSegmentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPathSegmentFeatureData.html), [IPrimaryMemberPointLengthFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData.html), [IPrimaryMemberRefPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData.html), [IPrimaryStructuralMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryStructuralMemberFeatureData.html), [IProfileGroupFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder.html),
          [ISecondaryMemberBetweenPointsFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData.html), [ISecondaryMemberSupportPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberSupportPlaneFeatureData.html), [ISecondaryStructuralMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryStructuralMemberFeatureData.html), [IStructureSystemMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData.html), [IStructureSystemMemberProfile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile.html), and [IStructureSystemSplitMember](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember.html).+ Graphics mesh and mesh BREP bodies. See [IBody2::GetGraphicsBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetGraphicsBody.html), [IBody2::GetMeshBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMeshBody.html), [IBody2::IsGraphicsBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsGraphicsBody.html), [IGraphicsBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody.html), [IMeshBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeshBody.html), and [IFacet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet.html).+ Scaled icons in the SOLIDWORKS add-in manager (**Tools > Add-ins...**) for third-party (Other) add-ins. See **SOLIDWORKS API Programming Guide >** **Getting Started > Programming with the SOLIDWORKS API > Add-ins > Icons**.

  * Redesign of:

    + Messages and alerts for add-ins. See [ISldWorks::DefineMessageBar](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~DefineMessageBar.html), [IModelDocExtension::ShowMessageBar](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ShowMessageBar.html), [IModelDocExtension::CloseMessageBar](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CloseMessageBar.html), [ISldWorks::DefineUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~DefineUserNotification.html), [IModelDocExtension::ShowUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ShowUserNotification.html), [ISldWorks::ShowUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ShowUserNotification.html), [IModelDocExtension::CloseUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CloseUserNotification.html), [ISldWorks::CloseUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CloseUserNotification.html), [IUserNotificationDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition.html), [IMessageBarDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition.html), IMessageBarHandler, and IUserNotificationHandler.+ Sheet metal corner relief feature:
        - Create feature using [IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html) and [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html).
        - See [ICornerReliefFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html) and [ISMCornerReliefData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData.html).+ Sheet metal base flange feature:
          - Create feature using IFeatureManager::CreateDefinition and IFeatureManager::CreateFeature.- See the new methods and properties in [IBaseFlangeFeatureData](#baseflangefeaturedata).- Obsoletes IFeatureManager::InsertSheetMetalBaseFlange2.

#### Other major enhancements

* Replace a sketch entity with construction and/or contour geometry. See [ISketchManager::SketchReplace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchReplace2.html).* Get all of the decals applied to a component face in an assembly. See [IFace2::GetAllAssemblyDecalProperties](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~GetAllAssemblyDecalProperties.html).* Get and set drawing sheet zone parameters. See [ISheet::GetZoneMargin](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetZoneMargin.html), [ISheet::GetZoneSizeDistribution](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetZoneSizeDistribution.html), [ISheet::GetZoneSizeRegion](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetZoneSizeRegion.html), [ISheet::SetZoneMargin](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetZoneMargin.html), [ISheet::SetZoneSizeDistribution](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetZoneSizeDistribution.html), and [ISheet::SetZoneSizeRegion](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetZoneSizeRegion.html).* Get angular ordinate dimension information from the current drawing sheet or view. See [IView::GetDimensionInfo7](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDimensionInfo7.html).* Restore default values of Hole Wizard hole or slot feature data. See [IWizardHoleFeatureData2::RestoreDefaultValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2~RestoreDefaultValues.html).* Upgrade legacy custom properties. See [IModelDocExtension::UpgradeLegacyCustomProperties](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpgradeLegacyCustomProperties.html).* Create a coordinate system based on position and orientation relative to the global coordinate system. See [IFeatureManager::CreateCoordinateSystemUsingNumericalValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateCoordinateSystemUsingNumericalValues.html).* Add doubled distance dimensions and toggle between single and doubled distance dimensions. See [IModelDocExtension::AddSpecificDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddSpecificDimension.html) and [IDisplayDimension::Diametric](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~Diametric.html).* Get and set whether to use the properties of the material applied when creating a new sheet metal feature. See [ISheetMetalFeatureData::UseMaterialSheetMetalParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData~UseMaterialSheetMetalParameters.html).* Close and reopen a specified drawing document with an ExitDetailingMode option. See [ISldWorks::CloseAndReopen2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CloseAndReopen2.html).* Reload or replace a model document with a force reload option. See [IModelDocExtension::ReloadOrReplace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ReloadOrReplace.html).* Prompt users for the name of the file to open with options. See [ISldWorks::GetOpenFileName2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetOpenFileName2.html).* For SOLIDWORKS Connected only:
                          + Add newPhysical Products and Representations (configurations) to a SOLIDWORKS Connected model. See [IConfiguration::Set3DExperienceType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Set3DExperienceType.html).+ Convert between parent and derived configurations. See [IConfiguration::Set3DExperienceType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Set3DExperienceType.html).+ Get and set whether a Representation configuration is shared. See [IConfiguration::RepresentationShared](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~RepresentationShared.html).+ Add and replace assembly components from a 3DEXPERIENCE collaborative space. See [IAssemblyDoc::AddPLMComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddPLMComponent.html) and [IAssemblyDoc::ReplacePLMComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReplacePLMComponents.html).

[Back to top](#Top)

###### New interfaces

#### [IBeltChainFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData.html) Interface

* [IBeltChainFeatureData::AccessBeltPart](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~AccessBeltPart.html)* [IBeltChainFeatureData::AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~AccessSelections.html)* [IBeltChainFeatureData::BeltLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~BeltLength.html)* [IBeltChainFeatureData::BeltLocationPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~BeltLocationPlane.html)* [IBeltChainFeatureData::BeltThickness](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~BeltThickness.html)* [IBeltChainFeatureData::CreateBeltPart](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~CreateBeltPart.html)* [IBeltChainFeatureData::DrivingLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~DrivingLength.html)* [IBeltChainFeatureData::EngageBelt](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~EngageBelt.html)* [IBeltChainFeatureData::FlipSides](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~FlipSides.html)* [IBeltChainFeatureData::GetMemberIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~GetMemberIndex.html)* [IBeltChainFeatureData::ModifyMemberParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~ModifyMemberParameters.html)* [IBeltChainFeatureData::PulleyComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~PulleyComponents.html)* [IBeltChainFeatureData::PulleyDiameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~PulleyDiameters.html)* [IBeltChainFeatureData::ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~ReleaseSelectionAccess.html)* [IBeltChainFeatureData::UseBeltThickness](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~UseBeltThickness.html)

#### [ICornerReliefFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html) Interface

* [ICornerReliefFeatureData::AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~AccessSelections.html)* [ICornerReliefFeatureData::AddNewCorner](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~AddNewCorner.html)* [ICornerReliefFeatureData::CollectAllCorners](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~CollectAllCorners.html)* [ICornerReliefFeatureData::CornerCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~CornerCount.html)* [ICornerReliefFeatureData::CornerType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~CornerType.html)* [ICornerReliefFeatureData::GetBodyScope](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~GetBodyScope.html)* [ICornerReliefFeatureData::GetCornerAtIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~GetCornerAtIndex.html)* [ICornerReliefFeatureData::GetCorners](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~GetCorners.html)* [ICornerReliefFeatureData::Initialize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~Initialize.html)* [ICornerReliefFeatureData::ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~ReleaseSelectionAccess.html)* [ICornerReliefFeatureData::RemoveCorner](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~RemoveCorner.html)* [ICornerReliefFeatureData::SetBodyScope](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~SetBodyScope.html)

#### [IFacet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet.html) Interface

* [IFacet::GetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet~GetBody.html)* [IFacet::GetFacetEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet~GetFacetEdges.html)* [IFacet::GetFacetVertices](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet~GetFacetVertices.html)* [IFacet::Select](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet~Select.html)

#### [IGraphicsBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody.html) Interface

* [IGraphicsBody::GetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody.html)* [IGraphicsBody::GetFacetCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody~GetFacetCount.html)* [IGraphicsBody::GetFacets](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody~GetFacets.html)

#### [IMeshBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeshBody.html) Interface

* [IMeshBody::GetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeshBody~GetBody.html)* [IMeshBody::GetFacetCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeshBody~GetFacetCount.html)* [IMeshBody::GetFacets](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeshBody~GetFacets.html)

#### [IMessageBarDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition.html) Interface

* [IMessageBarDefinition::IncludeDoNotShowAgain](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition~IncludeDoNotShowAgain.html)* [IMessageBarDefinition::Message](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition~Message.html)* [IMessageBarDefinition::ResponseAText](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition~ResponseAText.html)* [IMessageBarDefinition::ResponseAType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition~ResponseAType.html)* [IMessageBarDefinition::ResponseBText](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition~ResponseBText.html)* [IMessageBarDefinition::ResponseBType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition~ResponseBType.html)* [IMessageBarDefinition::Severity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition~Severity.html)* [IMessageBarDefinition::Title](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition~Title.html)* [IMessageBarDefinition::UniqueName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition~UniqueName.html)

#### [IPrimaryMemberFacePlaneIntersectionFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData.html) Interface

* [IPrimaryMemberFacePlaneIntersectionFeatureData::GetIntersectingObjectTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData~GetIntersectingObjectTypes.html)* [IPrimaryMemberFacePlaneIntersectionFeatureData::GetIntersectingPlanesAndFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData~GetIntersectingPlanesAndFaces.html)* [IPrimaryMemberFacePlaneIntersectionFeatureData::GetParameterFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData~GetParameterFaces.html)* [IPrimaryMemberFacePlaneIntersectionFeatureData::MergeTangentMembers](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData~MergeTangentMembers.html)* [IPrimaryMemberFacePlaneIntersectionFeatureData::SetIntersectingPlanesAndFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData~SetIntersectingPlanesAndFaces.html)* [IPrimaryMemberFacePlaneIntersectionFeatureData::SetParameterFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData~SetParameterFaces.html)

#### [IPrimaryMemberPathSegmentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPathSegmentFeatureData.html) Interface

* [IPrimaryMemberPathSegmentFeatureData::GetPathSegments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPathSegmentFeatureData~GetPathSegments.html)* [IPrimaryMemberPathSegmentFeatureData::GetPathSegmentsTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPathSegmentFeatureData~GetPathSegmentsTypes.html)* [IPrimaryMemberPathSegmentFeatureData::MergeTangentMembers](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPathSegmentFeatureData~MergeTangentMembers.html)* [IPrimaryMemberPathSegmentFeatureData::SetPathSegments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPathSegmentFeatureData~SetPathSegments.html)

#### [IPrimaryMemberPointLengthFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData.html) Interface

* [IPrimaryMemberPointLengthFeatureData::DirectionReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~DirectionReference.html)* [IPrimaryMemberPointLengthFeatureData::EndCondition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~EndCondition.html)* [IPrimaryMemberPointLengthFeatureData::EndPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~EndPlane.html)* [IPrimaryMemberPointLengthFeatureData::EndPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~EndPoint.html)

* [IPrimaryMemberPointLengthFeatureData::GetPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~GetPoints.html)* [IPrimaryMemberPointLengthFeatureData::GetPointsTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~GetPointsTypes.html)* [IPrimaryMemberPointLengthFeatureData::Length](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~Length.html)* [IPrimaryMemberPointLengthFeatureData::ReverseDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~ReverseDirection.html)* [IPrimaryMemberPointLengthFeatureData::SetPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~SetPoints.html)* [IPrimaryMemberPointLengthFeatureData::UnChainPointsAndLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData~UnChainPointsAndLength.html)

#### [IPrimaryMemberRefPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData.html) Interface

* [IPrimaryMemberRefPlaneFeatureData::GetReferenceAxes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData~GetReferenceAxes.html)* [IPrimaryMemberRefPlaneFeatureData::GetReferenceAxesTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData~GetReferenceAxesTypes.html)* [IPrimaryMemberRefPlaneFeatureData::GetReferenceLocations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData~GetReferenceLocations.html)* [IPrimaryMemberRefPlaneFeatureData::GetReferenceLocationsTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData~GetReferenceLocationsTypes.html)* [IPrimaryMemberRefPlaneFeatureData::GetStartAndEndReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData~GetStartAndEndReferences.html)* [IPrimaryMemberRefPlaneFeatureData::GetStartAndEndReferencesTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData~GetStartAndEndReferencesTypes.html)* [IPrimaryMemberRefPlaneFeatureData::SetReferenceAxes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData~SetReferenceAxes.html)* [IPrimaryMemberRefPlaneFeatureData::SetReferenceLocations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData~SetReferenceLocations.html)* [IPrimaryMemberRefPlaneFeatureData::SetStartAndEndReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData~SetStartAndEndReferences.html)

#### [IPrimaryStructuralMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryStructuralMemberFeatureData.html) Interface

* [IPrimaryStructuralMemberFeatureData::PrimaryMemberType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryStructuralMemberFeatureData~PrimaryMemberType.html)

#### [IProfileGroupFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder.html) Interface

* [IProfileGroupFolder::GetFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~GetFeature.html)* [IProfileGroupFolder::GetPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~GetPlane.html)* [IProfileGroupFolder::GetSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~GetSketch.html)* [IProfileGroupFolder::GetStructureSystemMemberCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~GetStructureSystemMemberCount.html)* [IProfileGroupFolder::GetStructureSystemMembers](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~GetStructureSystemMembers.html)* [IProfileGroupFolder::ProfileSize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~ProfileSize.html)* [IProfileGroupFolder::ProfileStandard](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~ProfileStandard.html)* [IProfileGroupFolder::ProfileType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~ProfileType.html)

#### [ISecondaryMemberBetweenPointsFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData.html) Interface

* [ISecondaryMemberBetweenPointsFeatureData::GetMemberPairs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~GetMemberPairs.html)* [ISecondaryMemberBetweenPointsFeatureData::DistanceMember1](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~DistanceMember1.html)* [ISecondaryMemberBetweenPointsFeatureData::DistanceMember2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~DistanceMember2.html)* [ISecondaryMemberBetweenPointsFeatureData::LengthRatioMember1](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~LengthRatioMember1.html)* [ISecondaryMemberBetweenPointsFeatureData::LengthRatioMember2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~LengthRatioMember2.html)* [ISecondaryMemberBetweenPointsFeatureData::RevDirectionDistanceMember1](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~RevDirectionDistanceMember1.html)* [ISecondaryMemberBetweenPointsFeatureData::RevDirectionDistanceMember2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~RevDirectionDistanceMember2.html)* [ISecondaryMemberBetweenPointsFeatureData::RevDirectionLengthRatioMember1](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~RevDirectionLengthRatioMember1.html)* [ISecondaryMemberBetweenPointsFeatureData::RevDirectionLengthRatioMember2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~RevDirectionLengthRatioMember2.html)* [ISecondaryMemberBetweenPointsFeatureData::SecondaryMemberOffsetType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~SecondaryMemberOffsetType.html)* [ISecondaryMemberBetweenPointsFeatureData::SetMemberPairs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~SetMemberPairs.html)* [ISecondaryMemberBetweenPointsFeatureData::UnChainMemberPairs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~UnChainMemberPairs.html)

#### [ISecondaryMemberSupportPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberSupportPlaneFeatureData.html) Interface

* [ISecondaryMemberSupportPlaneFeatureData::GetIntersectingObjectTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberSupportPlaneFeatureData~GetIntersectingObjectTypes.html)* [ISecondaryMemberSupportPlaneFeatureData::GetIntersectingPlanesAndFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberSupportPlaneFeatureData~GetIntersectingPlanesAndFaces.html)* [ISecondaryMemberSupportPlaneFeatureData::GetMemberPairs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberSupportPlaneFeatureData~GetMemberPairs.html)* [ISecondaryMemberSupportPlaneFeatureData::SetIntersectingPlanesAndFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberSupportPlaneFeatureData~SetIntersectingPlanesAndFaces.html)* [ISecondaryMemberSupportPlaneFeatureData::SetMemberPairs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberSupportPlaneFeatureData~SetMemberPairs.html)* [ISecondaryMemberSupportPlaneFeatureData::UnChainMemberPairs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberSupportPlaneFeatureData~UnChainMemberPairs.html)

#### [ISecondaryStructuralMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryStructuralMemberFeatureData.html) Interface

* [ISecondaryStructuralMemberFeatureData::SecondaryMemberType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryStructuralMemberFeatureData~SecondaryMemberType.html)

#### [ISMCornerReliefData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData.html) Interface

* [ISMCornerReliefData::AddFilletedCorners](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~AddFilletedCorners.html)* [ISMCornerReliefData::CenterOnBendLines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~CenterOnBendLines.html)* [ISMCornerReliefData::CornerFilletDiameter](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~CornerFilletDiameter.html)* [ISMCornerReliefData::CornerIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~CornerIndex.html)* [ISMCornerReliefData::GetFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~GetFaces.html)* [ISMCornerReliefData::RatioToThickness](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~RatioToThickness.html)* [ISMCornerReliefData::ReliefType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~ReliefType.html)* [ISMCornerReliefData::SlotLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~SlotLength.html)* [ISMCornerReliefData::SlotWidth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~SlotWidth.html)* [ISMCornerReliefData::SuitCaseType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~SuitCaseType.html)* [ISMCornerReliefData::TangentToBend](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~TangentToBend.html)

#### [IStructureSystemFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder.html) Interface

* [IStructureSystemFolder::GetFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder~GetFeature.html)* [IStructureSystemFolder::GetProfileGroupFolders](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder~GetProfileGroupFolders.html)* [IStructureSystemFolder::GetProfileGroupFoldersCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder~GetProfileGroupFoldersCount.html)

#### [IStructureSystemMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData.html) Interface

* [IStructureSystemMemberFeatureData::AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~AccessSelections.html)* [IStructureSystemMemberFeatureData::GetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~GetBody.html)* [IStructureSystemMemberFeatureData::GetFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~GetFeature.html)* [IStructureSystemMemberFeatureData::MemberProfile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~MemberProfile.html)* [IStructureSystemMemberFeatureData::ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~ReleaseSelectionAccess.html)* [IStructureSystemMemberFeatureData::StartEndExtendD1](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~StartEndExtendD1.html)* [IStructureSystemMemberFeatureData::StartEndExtendD2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~StartEndExtendD2.html)* [IStructureSystemMemberFeatureData::StructureSystemMemberType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~StructureSystemMemberType.html)

#### [IStructureSystemMemberProfile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile.html) Interface

* [IStructureSystemMemberProfile::GetSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~GetSketch.html)* [IStructureSystemMemberProfile::MirrorProfile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~MirrorProfile.html)* [IStructureSystemMemberProfile::OffsetPiercePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~OffsetPiercePoint.html)* [IStructureSystemMemberProfile::OffsetPiercePointHorizontalAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~OffsetPiercePointHorizontalAxis.html)* [IStructureSystemMemberProfile::OffsetPiercePointHorizontalAxisFlip](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~OffsetPiercePointHorizontalAxisFlip.html)* [IStructureSystemMemberProfile::OffsetPiercePointVerticalAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~OffsetPiercePointVerticalAxis.html)* [IStructureSystemMemberProfile::OffsetPiercePointVerticalAxisFlip](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~OffsetPiercePointVerticalAxisFlip.html)* [IStructureSystemMemberProfile::PiercePointSelectionObject](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~PiercePointSelectionObject.html)* [IStructureSystemMemberProfile::ProfileAlignmentAngle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~ProfileAlignmentAngle.html)* [IStructureSystemMemberProfile::ProfileAlignmentObject](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~ProfileAlignmentObject.html)* [IStructureSystemMemberProfile::ProfileAlignmentObjectType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~ProfileAlignmentObjectType.html)* [IStructureSystemMemberProfile::ProfileAlignmentType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~ProfileAlignmentType.html)* [IStructureSystemMemberProfile::ProfileMirrorType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~ProfileMirrorType.html)* [IStructureSystemMemberProfile::ProfilePiercePointType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~ProfilePiercePointType.html)* [IStructureSystemMemberProfile::ProfileSize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~ProfileSize.html)* [IStructureSystemMemberProfile::ProfileStandard](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~ProfileStandard.html)* [IStructureSystemMemberProfile::ProfileType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile~ProfileType.html)

#### [IStructureSystemSplitMember](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember.html) Interface

* [IStructureSystemSplitMember::DimensionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember~DimensionType.html)* [IStructureSystemSplitMember::GetSplitReferenceObjectTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember~GetSplitReferenceObjectTypes.html)* [IStructureSystemSplitMember::GetSplitReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember~GetSplitReferences.html)* [IStructureSystemSplitMember::MemberType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember~MemberType.html)* [IStructureSystemSplitMember::NumberofSplitInstances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember~NumberofSplitInstances.html)* [IStructureSystemSplitMember::SetSplitReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember~GetSplitReferences.html)* [IStructureSystemSplitMember::SplitLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember~SplitLength.html)* [IStructureSystemSplitMember::SplitLengthRevDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember~SplitLengthRevDirection.html)

#### [IUserNotificationDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition.html) Interface

* [IUserNotificationDefinition::IncludeDoNotShowAgain](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~IncludeDoNotShowAgain.html)* [IUserNotificationDefinition::Message](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~Message.html)* [IUserNotificationDefinition::Position](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~Position.html)* [IUserNotificationDefinition::ResponseAText](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~ResponseAText.html)* [IUserNotificationDefinition::ResponseAType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~ResponseAType.html)* [IUserNotificationDefinition::ResponseBText](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~ResponseBText.html)* [IUserNotificationDefinition::ResponseBType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~ResponseBType.html)* [IUserNotificationDefinition::Severity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~Severity.html)* [IUserNotificationDefinition::Title](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~Title.html)* [IUserNotificationDefinition::UniqueName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition~UniqueName.html)

New SOLIDWORKS Custom Interfaces

#### IMessageBarHandler Interface

* IMessageBarHandler::OnUserClose* IMessageBarHandler::OnUserResponseA* IMessageBarHandler::OnUserResponseB

#### IUserNotificationHandler Interface

* IUserNotificationHandler::OnTimeout* IUserNotificationHandler::OnUserClose* IUserNotificationHandler::OnUserResponseA* IUserNotificationHandler::OnUserResponseB

[Back to top](#Top)

###### New methods, properties, and delegates

#### IAssemblyDoc Interface

* [IAssemblyDoc::AddPLMComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddPLMComponent.html)* [IAssemblyDoc::ReplacePLMComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReplacePLMComponents.html)

#### IBaseFlangeFeatureData Interface

* [IBaseFlangeFeatureData::D1EndConditionDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D1EndConditionDistance.html) (obsoletes IBaseFlangeFeatureData::D1OffsetDistance)* [IBaseFlangeFeatureData::D1EndConditionReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D1EndConditionReference.html) (obsoletes IBaseFlangeFeatureData::D1OffsetReference)* [IBaseFlangeFeatureData::D1EndConditionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D1EndConditionType.html) (obsoletes IBaseFlangeFeatureData::D1OffsetType)* [IBaseFlangeFeatureData::D2EndConditionDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D2EndConditionDistance.html) (obsoletes IBaseFlangeFeatureData::D2OffsetDistance)* [IBaseFlangeFeatureData::D2EndConditionReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D2EndConditionReference.html) (obsoletes IBaseFlangeFeatureData::D2OffsetReference)* [IBaseFlangeFeatureData::D2EndConditionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D2EndConditionType.html) (obsoletes IBaseFlangeFeatureData::D2OffsetType)* [IBaseFlangeFeatureData::GetCustomBendAllowance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~GetCustomBendAllwance.html)* [IBaseFlangeFeatureData::Initialize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~Initialize.html)* [IBaseFlangeFeatureData::OverrideDefaultSheetMetalParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~OverrideDefaultSheetMetalParameters.html)* [IBaseFlangeFeatureData::ReliefDepth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~ReliefDepth.html)* [IBaseFlangeFeatureData::ReliefRatio](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~ReliefRatio.html)* [IBaseFlangeFeatureData::ReliefType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~ReliefType.html)* [IBaseFlangeFeatureData::ReliefWidth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~ReliefWidth.html)* [IBaseFlangeFeatureData::UseDefaultBendAllowance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~UseDefaultBendAllowance.html)* [IBaseFlangeFeatureData::UseDefaultBendRelief](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~UseDefaultBendRelief.html)* [IBaseFlangeFeatureData::UseMaterialSheetMetalParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~UseMaterialSheetMetalParameters.html)* [IBaseFlangeFeatureData::UseReliefRatio](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~UseReliefRatio.html)

#### IBody2 Interface

* [IBody2::GetGraphicsBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetGraphicsBody.html)* [IBody2::GetMeshBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMeshBody.html)* [IBody2::IsGraphicsBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsGraphicsBody.html)

#### IConfiguration Interface

* [IConfiguration::RepresentationShared](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~RepresentationShared.html)* [IConfiguration::Set3DExperienceType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Set3DExperienceType.html)

#### IConfigurationManager Interface

* [IConfigurationManager::AddCADFamilyConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddCADFamilyConfiguration.html)

#### IFace2 Interface

* [IFace2::GetAllAssemblyDecalProperties](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~GetAllAssemblyDecalProperties.html)

#### IFeatureManager Interface

* [IFeatureManager::CreateCoordinateSystemUsingNumericalValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateCoordinateSystemUsingNumericalValues.html)* [IFeatureManager::GetStructureSystemFolders](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~GetStructureSystemFolders.html)

#### IModelDocExtension Interface

* [IModelDocExtension::CloseMessageBar](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CloseMessageBar.html)* [IModelDocExtension::CloseUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CloseUserNotification.html)* [IModelDocExtension::CreateStructureSystem](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateStructureSystem.html)* [IModelDocExtension::CreateStructureSystemMemberData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateStructureSystemMemberData.html)* [IModelDocExtension::ReloadOrReplace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ReloadOrReplace.html) (obsoletes IModelDoc2::ReloadOrReplace)* [IModelDocExtension::ShowMessageBar](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ShowMessageBar.html)* [IModelDocExtension::ShowUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ShowUserNotification.html)* [IModelDocExtension::UpgradeLegacyCustomProperties](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpgradeLegacyCustomProperties.html)

#### ISheet Interface

* [ISheet::GetZoneMargin](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetZoneMargin.html)* [ISheet::GetZoneSizeDistribution](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetZoneSizeDistribution.html)* [ISheet::GetZoneSizeRegion](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetZoneSizeRegion.html)* [ISheet::SetZoneMargin](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetZoneMargin.html)* [ISheet::SetZoneSizeDistribution](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetZoneSizeDistribution.html)* [ISheet::SetZoneSizeRegion](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetZoneSizeRegion.html)

#### ISheetMetalFeatureData Interface

* [ISheetMetalFeatureData::UseMaterialSheetMetalParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData~UseMaterialSheetMetalParameters.html)

#### ISketchManager Interface

* [ISketchManager::SketchReplace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchReplace2.html) (obsoletes ISketchManager::SketchReplace)

#### ISldWorks Interface

* [ISldWorks::CloseAndReopen2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CloseAndReopen2.html) (obsoletes ISldWorks::CloseAndReopen)* [ISldWorks::CloseUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CloseUserNotification.html)* [ISldWorks::DefineMessageBar](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~DefineMessageBar.html)* [ISldWorks::DefineUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~DefineUserNotification.html)* [ISldWorks::GetOpenFileName2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetOpenFileName2.html) (obsoletes ISldWiorks::GetOpenFileName)* [ISldWorks::LoadAdminSettingsFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~LoadAdminSettingsFile.html)* [ISldWorks::ShowUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ShowUserNotification.html)

#### IView Interface

* [IView::GetDimensionInfo7](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDimensionInfo7.html) (obsoletes IView::GetDimensionInfo6 and IView::IGetDimensionInfo6)

#### IWizardHoleFeatureData2 Interface

* [IWizardHoleFeatureData2::RestoreDefaultValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2~RestoreDefaultValues.html)

[Back to top](#Top)

###### Obsoleted methods and properties

#### IBaseFlangeFeatureData Interface

* IBaseFlangeFeatureData::D1OffsetDistance (superseded by [IBaseFlangeFeatureData::D1EndConditionDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D1EndConditionDistance.html))* IBaseFlangeFeatureData::D1OffsetReference (superseded by [IBaseFlangeFeatureData::D1EndConditionReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D1EndConditionReference.html))* IBaseFlangeFeatureData::D1OffsetType (superseded by [IBaseFlangeFeatureData::D1EndConditionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D1EndConditionType.html))* IBaseFlangeFeatureData::D2OffsetDistance (superseded by [IBaseFlangeFeatureData::D2EndConditionDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D2EndConditionDistance.html))* IBaseFlangeFeatureData::D2OffsetReference (superseded by [IBaseFlangeFeatureData::D2EndConditionReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D2EndConditionReference.html))* IBaseFlangeFeatureData::D2OffsetType (superseded by [IBaseFlangeFeatureData::D2EndConditionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~D2EndConditionType.html))

#### IFeatureManager Interface

* IFeatureManager::InsertSheetMetalBaseFlange2 (superseded by [IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html), [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html), and [IBaseFlangeFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData.html))

#### IModelDoc2 Interface

* IModelDoc2::ReloadOrReplace (superseded by [IModelDocExtension::ReloadOrReplace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ReloadOrReplace.html)).

#### ISketchManager Interface

* ISketchManager::SketchReplace (superseded by [ISketchManager::SketchReplace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchReplace2.html))

#### ISldWorks Interface

* ISldWorks::CloseAndReopen (superseded by [ISldWorks::CloseAndReopen2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CloseAndReopen2.html))* ISldWorks::GetOpenFileName (superseded by [ISldWorks::GetOpenFileName2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetOpenFileName2.html))

#### IView Interface

* IView::GetDimensionInfo6 and IView::IGetDimensionInfo6 (superseded by [IView::GetDimensionInfo7](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDimensionInfo7.html))

[Back to top](#Top)