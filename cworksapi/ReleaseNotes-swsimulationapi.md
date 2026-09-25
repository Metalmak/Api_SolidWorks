<!-- source: cworksapi/ReleaseNotes-swsimulationapi.html -->

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
| SOLIDWORKS Simulation API Help |  |
| Release Notes |
| Send Feedback | |

Glossary Item Box

This topic provides you with quick access to the enhancements in SOLIDWORKS Simulation API 2022.

##### Service Pack 1

###### New method and property

#### ICWContactComponent interface

* [ICWContactComponent::BondingFormulation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~BondingFormulation.html)

#### ICWMultipleComponentContactsEditManager interface

* [ICWMultipleComponentContactsEditManager::SetBondingFormulation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~SetBondingFormulation.html)

##### Service Pack 0

This release continues comprehensive changes begun in SOLIDWORKS Simulation API 2021 SP04. Certain methods and properties now require VARIANT\_BOOL parameters and values. (VARIANT\_TRUE = -1, VARIANT\_FALSE = 0). You can run the sample code from previous releases in this release, but you will first need to replace the properties and methods in those examples with the properties and methods that use VARIANT\_BOOLs. Similarly, to work with this release your applications will need to be modified to use the new properties and methods that use VARIANT\_BOOLs. See the **New methods and properties** section below.

###### New interfaces

#### [ICWLinkageRod](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html) interface

* [ICWLinkageRod::BeginEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~BeginEdit.html)* [ICWLinkageRod::EndEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~EndEdit.html)* [ICWLinkageRod::GetLastErrorCode](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~GetLastErrorCode.html)* [ICWLinkageRod::IncludeMass](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~IncludeMass.html)* [ICWLinkageRod::InsertEntityAtEnd1](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~InsertEntityAtEnd1.html)* [ICWLinkageRod::InsertEntityAtEnd2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~InsertEntityAtEnd2.html)* [ICWLinkageRod::Mass](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~Mass.html)* [ICWLinkageRod::MaterialSource](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~MaterialSource.html)* [ICWLinkageRod::PoissonsRatio](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~PoissonsRatio.html)* [ICWLinkageRod::ReplaceEntitiesAtEnd1](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~ReplaceEntitiesAtEnd1.html)* [ICWLinkageRod::ReplaceEntitiesAtEnd2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~ReplaceEntitiesAtEnd2.html)* [ICWLinkageRod::SetFlipOffsetDirAtEnd1](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetFlipOffsetDirAtEnd1.html)* [ICWLinkageRod::SetFlipOffsetDirAtEnd2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetFlipOffsetDirAtEnd2.html)* [ICWLinkageRod::SetJointTypeAtEnd1](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetJointTypeAtEnd1.html)* [ICWLinkageRod::SetJointTypeAtEnd2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetJointTypeAtEnd2.html)* [ICWLinkageRod::SetLibraryMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetLibraryMaterial.html)* [ICWLinkageRod::SetOffsetAtEnd1](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetOffsetAtEnd1.html)* [ICWLinkageRod::SetOffsetAtEnd2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetOffsetAtEnd2.html)* [ICWLinkageRod::SetSectionParams](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetSectionParams.html)* [ICWLinkageRod::ThermalCoefficient](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~ThermalCoefficient.html)* [ICWLinkageRod::UnitType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~UnitType.html)* [ICWLinkageRod::YoungsModulus](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~YoungsModulus.html)

###### New methods and properties

#### ICWBaseExcitation interface

* [ICWBaseExcitation::GetExcitationDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections2.html) (obsoletes ICWBaseExcitation::GetExcitationDirections)* [ICWBaseExcitation::GetExcitationReverseDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationReverseDirections2.html) (obsoletes ICWBaseExcitation::GetExcitationReverseDirections)* [ICWBaseExcitation::SetExcitationDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationDirections2.html) (obsoletes ICWBaseExcitation::SetExcitationDirections)* [ICWBaseExcitation::SetExcitationReverseDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationReverseDirections2.html) (obsoletes ICWBaseExcitation::SetExcitationReverseDirections)* [ICWBaseExcitation::SetTimeOrFrequencyCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetTimeOrFrequencyCurve2.html) (obsoletes ICWBaseExcitation::SetTimeOrFrequencyCurve)

#### ICWBeamBody interface

* [ICWBeamBody::GetManualEnd1ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd1ConnectionType2.html) (obsoletes ICWBeamBody::GetManualEnd1ConnectionType)* [ICWBeamBody::GetManualEnd2ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd2ConnectionType2.html) (obsoletes ICWBeamBody::GetManualEnd2ConnectionType)* [ICWBeamBody::SetFavMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetFavMaterial2.html) (obsoletes ICWBeamBody::SetFavMaterial)* [ICWBeamBody::SetLibraryMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetLibraryMaterial2.html) (obsoletes ICWBeamBody::SetLibraryMaterial)* [ICWBeamBody::SetManualEnd1ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd1ConnectionType2.html) (obsoletes ICWBeamBody::SetManualEnd1ConnectionType)* [ICWBeamBody::SetManualEnd2ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd2ConnectionType2.html) (obsoletes ICWBeamBody::SetManualEnd2ConnectionType)

#### ICWBearingLoad interface

* [ICWBearingLoad::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~SetTimeCurve2.html) (obsoletes ICWBearingLoad::SetTimeCurve)* [ICWBearingLoad::UseTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~UseTimeCurve2.html) (obsoletes ICWBearingLoad::UseTimeCurve)* [ICWBearingLoad::XDirectionReverse2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~XDirectionReverse2.html) (obsoletes ICWBearingLoad::XDirectionReverse)* [ICWBearingLoad::YDirectionReverse2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~YDirectionReverse2.html) (obsoletes ICWBearingLoad::YDirectionReverse)

#### ICWBoltConnector interface

* [ICWBoltConnector::AllowDistributedCoupling2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector~AllowDistributedCoupling2.html) (obsoletes ICWBoltConnector::AllowDistributedCoupling)

#### ICWBucklingStudyOptions interface

* [ICWBucklingStudyOptions::CheckFlowPressure2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBucklingStudyOptions~CheckFlowPressure2.html) (obsoletes ICWBucklingStudyOptions::CheckFlowPressure)* [ICWBucklingStudyOptions::CheckRunAsLegacy2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBucklingStudyOptions~CheckRunAsLegacy2.html) (obsoletes ICWBucklingStudyOptions::CheckRunAsLegacy)* [ICWBucklingStudyOptions::Email2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBucklingStudyOptions~EMail2.html) (obsoletes ICWBucklingStudyOptions::Email)* [ICWBucklingStudyOptions::EmailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBucklingStudyOptions~EMailTimebased2.html) (obsoletes ICWBucklingStudyOptions::EmailTimebased)* [ICWBucklingStudyOptions::UseSoftSpring2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBucklingStudyOptions~UseSoftSpring2.html) (obsoletes ICWBucklingStudyOptions::UseSoftSpring)

#### ICWCentrifugalForce interface

* [ICWCentrifugalForce::ReverseAngAccelerationDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce~ReverseAngAccelerationDirection2.html) (obsoletes ICWCentrifugalForce::ReverseAngAccelerationDirection)* [ICWCentrifugalForce::ReverseAngVelocityDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce~ReverseAngVelocityDirection2.html) (obsoletes ICWCentrifugalForce::ReverseAngVelocityDirection)* [ICWCentrifugalForce::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce~SetTimeCurve2.html) (obsoletes ICWCentrifugalForce::SetTimeCurve)* [ICWCentrifugalForce::UseTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce~UseTimeCurve2.html) (obsoletes ICWCentrifugalForce::UseTimeCurve)

#### ICWCompositeShellOptions interface

* [ICWCompositeShellOptions::AllPliesSameMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~AllPliesSameMaterial2.html) (obsoletes ICWCompositeShellOptions::AllPliesSameMaterial)* [ICWCompositeShellOptions::GetMirrorOrientation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~GetMirrorOrientation2.html) (obsoletes ICWCompositeShellOptions::GetMirrorOrientation)* [ICWCompositeShellOptions::GetRotateOrientation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~GetRotateOrientation2.html) (obsoletes ICWCompositeShellOptions::GetRotateOrientation)* [ICWCompositeShellOptions::PlyRelativeAngle2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~PlyRelativeAngle2.html) (obsoletes ICWCompositeShellOptions::PlyRelativeAngle)* [ICWCompositeShellOptions::RotateZeroDegreeReference2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~RotateZeroDegreeReference2.html) (obsoletes ICWCompositeShellOptions::RotateZeroDegreeReference)* [ICWCompositeShellOptions::Sandwich2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~Sandwich2.html) (obsoletes ICWCompositeShellOptions::Sandwich)* [ICWCompositeShellOptions::SetMirrorOrientation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~SetMirrorOrientation2.html) (obsoletes ICWCompositeShellOptions::SetMirrorOrientation)* [ICWCompositeShellOptions::SetRotateOrientation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~SetRotateOrientation2.html) (obsoletes ICWCompositeShellOptions::SetRotateOrientation)* [ICWCompositeShellOptions::Symmetric2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~Symmetric2.html) (obsoletes ICWCompositeShellOptions::Symmetric)

#### ICWContactComponent interface

* [ICWContactComponent::GlobalContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~GlobalContact2.html) (obsoletes ICWContactComponent::GlobalContact)* [ICWContactComponent::IncludeClearance2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeClearance2.html) (obsoletes ICWContactComponent::IncludeClearance)* [ICWContactComponent::IncludeFriction2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeFriction2.html) (obsoletes ICWContactComponent::IncludeFriction)* [ICWContactComponent::IncludeShellEdgeSolidOrShellFace2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeShellEdgeSolidOrShellFace2.html) (obsoletes ICWContactComponent::IncludeShellEdgeSolidOrShellFace)

#### ICWContactManager interface

* [ICWContactManager::SuppressUnsuppressComponentContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressComponentContact2.html) (obsoletes ICWContactManager::SuppressUnsuppressComponentContact)* [ICWContactManager::SuppressUnsuppressContactPair2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressContactPair2.html) (obsoletes ICWContactManager::SuppressUnsuppressContactPair)

#### ICWContactSet interface

* [ICWContactSet::IncludeFriction2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~IncludeFriction2.html) (obsoletes ICWContactSet::IncludeFriction)

#### ICWConvection interface

* [ICWConvection::SetBulkTemperatureTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~SetBulkTemperatureTimeCurve2.html) (obsoletes ICWConvection::SetBulkTemperatureTimeCurve)* [ICWConvection::SetTemperatureCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~SetTemperatureCurve2.html) (obsoletes ICWConvection::SetTemperatureCurve)* [ICWConvection::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~SetTimeCurve2.html) (obsoletes ICWConvection::SetTimeCurve)* [ICWConvection::UseBulkTemperatureTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~UseBulkTemperatureTimeCurve2.html) (obsoletes ICWConvection::UseBulkTemperatureTimeCurve)* [ICWConvection::UseTemperatureCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~UseTemperatureCurve2.html) (obsoletes ICWConvection::UseTemperatureCurve)* [ICWConvection::UseTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~UseTimeCurve2.html) (obsoletes ICWConvection::UseTimeCurve)

#### ICWDampingOptions interface

* [ICWDampingOptions::ComputeFromMaterialDamping2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~ComputeFromMaterialDamping2.html) (obsoletes ICWDampingOptions::ComputeFromMaterialDamping)

#### ICWDropTestSetup interface

* [ICWDropTestSetup::FlipGravityDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup~FlipGravityDirection2.html) (obsoletes ICWDropTestSetup::FlipGravityDirection)* [ICWDropTestSetup::FlipVelocityDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup~FlipVelocityDirection2.html) (obsoletes ICWDropTestSetup::FlipVelocityDirection)* [ICWDropTestSetup::SetEntityForGravityDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup~SetEntityForGravityDirection2.html) (obsoletes ICWDropTestSetup::SetEntityForGravityDirection)* [ICWDropTestSetup::SetEntityForTargetOrientation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup~SetEntityForTargetOrientation2.html) (obsoletes ICWDropTestSetup::SetEntityForTargetOrientation)* [ICWDropTestSetup::SetEntityForVelocityDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup~SetEntityForVelocityDirection2.html) (obsoletes ICWDropTestSetup::SetEntityForVelocityDirection)

#### ICWDropTestStudyOptions interface

* [ICWDropTestStudyOptions::Email2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions~EMail2.html) (obsoletes ICWDropTestStudyOptions::Email)* [ICWDropTestStudyOptions::EmailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions~EMailTimebased2.html) (obsoletes ICWDropTestStudyOptions::EmailTimebased)* [ICWDropTestStudyOptions::LargeDisplacement2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions~LargeDisplacement2.html) (obsoletes ICWDropTestStudyOptions::LargeDisplacement)

#### ICWDynamicInitialCondition interface

* [ICWDynamicInitialCondition::GetDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetDirections2.html) (obsoletes ICWDynamicInitialCondition::GetDirections)* [ICWDynamicInitialCondition::GetReverseDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetReverseDirections2.html) (obsoletes ICWDynamicInitialCondition::GetReverseDirections)* [ICWDynamicInitialCondition::SetDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetDirections2.html) (obsoletes ICWDynamicInitialCondition::SetDirections)* [ICWDynamicInitialCondition::SetReverseDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetReverseDirections2.html) (obsoletes ICWDynamicInitialCondition::SetReverseDirections)

#### ICWDynamicStudyOptions interface

* [ICWDynamicStudyOptions::Email2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~EMail2.html) (obsoletes ICWDynamicStudyOptions::Email)* [ICWDynamicStudyOptions::EmailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~EMailTimebased2.html) (obsoletes ICWDynamicStudyOptions::EmailTimebased)* [ICWDynamicStudyOptions::GetResponseSpectrumUseMaterialDamping3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetResponseSpectrumUseMaterialDamping3.html) (obsoletes ICWDynamicStudyOptions::GetResponseSpectrumUseMaterialDamping2)* [ICWDynamicStudyOptions::GetUseSoftSpring3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetUseSoftSpring3.html) (obsoletes ICWDynamicStudyOptions::GetUseSoftSpring2)* [ICWDynamicStudyOptions::SetResponseSpectrumUseMaterialDamping3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetResponseSpectrumUseMaterialDamping3.html) (obsoletes ICWDynamicStudyOptions::SetResponseSpectrumUseMaterialDamping2)* [ICWDynamicStudyOptions::SetUseSoftSpring3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetUseSoftSpring3.html) (obsoletes ICWDynamicStudyOptions::SetUseSoftSpring2)

#### ICWFatigueStudyOptions interface

* [ICWFatigueStudyOptions::Email2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMail2.html) (obsoletes ICWFatigueStudyOptions::Email)* [ICWFatigueStudyOptions::EmailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~EMailTimebased2.html) (obsoletes ICWFatigueStudyOptions::EmailTimebased)* [ICWFatigueStudyOptions::GetInfiniteLifeSettings2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~GetInfiniteLifeSettings2.html) (obsoletes ICWFatigueStudyOptions::GetInfiniteLifeSettings)* [ICWFatigueStudyOptions::SetInfiniteLifeSettings2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~SetInfiniteLifeSettings2.html) (obsoletes ICWFatigueStudyOptions::SetInfiniteLifeSettings)

#### ICWForce interface

* [ICWForce::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetTimeCurve2.html) (obsoletes ICWForce::SetTimeCurve)

#### ICWFrequencyStudyOptions interface

* [ICWFrequencyStudyOptions::CheckFlowPressure2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions~CheckFlowPressure2.html) (obsoletes ICWFrequencyStudyOptions::CheckFlowPressure)* [ICWFrequencyStudyOptions::CheckRunAsLegacy2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions~CheckRunAsLegacy2.html) (obsoletes ICWFrequencyStudyOptions::CheckRunAsLegacy)* [ICWFrequencyStudyOptions::Email2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions~EMail2.html) (obsoletes ICWFrequencyStudyOptions::Email)* [ICWFrequencyStudyOptions::EmailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions~EMailTimebased2.html) (obsoletes ICWFrequencyStudyOptions::EmailTimebased)* [ICWFrequencyStudyOptions::UseLowerBoundFrequency2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions~UseLowerBoundFrequency2.html) (obsoletes ICWFrequencyStudyOptions::UseLowerBoundFrequency)* [ICWFrequencyStudyOptions::UseSoftSpring2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions~UseSoftSpring2.html) (obsoletes ICWFrequencyStudyOptions::UseSoftSpring)

#### ICWGravity interface

* [ICWGravity::ReverseDirectionAlongPlaneDir1\_2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionAlongPlaneDir1_2.html) (obsoletes ICWGravity::ReverseDirectionAlongPlaneDir1)* [ICWGravity::ReverseDirectionAlongPlaneDir2\_2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionAlongPlaneDir2_2.html) (obsoletes ICWGravity::ReverseDirectionAlongPlaneDir2)* [ICWGravity::ReverseDirectionNormalToPlane2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionNormalToPlane2.html) (obsoletes ICWGravity::ReverseDirectionNormalToPlane)

#### ICWHeatFlux interface

* [ICWHeatFlux::IncludeThermostat2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux~IncludeThermostat2.html) (obsoletes ICWHeatFlux::IncludeThermostat)* [ICWHeatFlux::PerUnitLength2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux~PerUnitLength2.html) (obsoletes ICWHeatFlux::PerUnitLength)* [ICWHeatFlux::ReverseDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux~ReverseDirection2.html) (obsoletes ICWHeatFlux::ReverseDirection)* [ICWHeatFlux::SetTemperatureCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux~SetTemperatureCurve2.html) (obsoletes ICWHeatFlux::SetTemperatureCurve)* [ICWHeatFlux::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux~SetTimeCurve2.html) (obsoletes ICWHeatFlux::SetTimeCurve)* [ICWHeatFlux::UseTemperatureCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux~UseTemperatureCurve2.html) (obsoletes ICWHeatFlux::UseTemperatureCurve)* [ICWHeatFlux::UseTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux~UseTimeCurve2.html) (obsoletes ICWHeatFlux::UseTimeCurve)

#### ICWHeatPower interface

* [ICWHeatPower::IncludeThermostat2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower~IncludeThermostat2.html) (obsoletes ICWHeatPower::IncludeThermostat)* [ICWHeatPower::ReverseDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower~ReverseDirection2.html) (obsoletes ICWHeatPower::ReverseDirection)* [ICWHeatPower::SetTemperatureCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower~SetTemperatureCurve2.html) (obsoletes ICWHeatPower::SetTemperatureCurve)* [ICWHeatPower::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower~SetTimeCurve2.html) (obsoletes ICWHeatPower::SetTimeCurve)* [ICWHeatPower::UseTemperatureCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower~UseTemperatureCurve2.html) (obsoletes ICWHeatPower::UseTemperatureCurve)* [ICWHeatPower::UseTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower~UseTimeCurve2.html) (obsoletes ICWHeatPower::UseTimeCurve)

#### ICWLoadsAndRestraintsManager interface

* [ICWLoadsAndRestraintsManager::AddInitialConditionForDynamicStudy2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddInitialConditionForDynamicStudy2.html) (obsoletes ICWLoadsAndRestraintsManager::AddInitialConditionForDynamicStudy)* [ICWLoadsAndRestraintsManager::AddLinkageRod](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddLinkageRod.html)* [ICWLoadsAndRestraintsManager::GetLinkageRod](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~GetLinkageRod.html)* [ICWLoadsAndRestraintsManager::AddSelectedBaseExcitation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddSelectedBaseExcitation2.html) (obsoletes ICWLoadsAndRestraintsManager::AddSelectedBaseExcitation)* [ICWLoadsAndRestraintsManager::AddUniformBaseExcitation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddUniformBaseExcitation2.html) (obsoletes ICWLoadsAndRestraintsManager::AddUniformBaseExcitation)

#### ICWMassPropertiesManager interface

* [ICWMassPropertiesManager::AddLinkageRods](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~AddLinkageRods.html)* [ICWMassPropertiesManager::RemoveAllLinkageRods](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~RemoveAllLinkageRods.html)* [ICWMassPropertiesManager::RemoveLinkageRods](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~RemoveLinkageRods.html)

#### ICWMaterial interface

* [ICWMaterial::IncludeCreep2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~IncludeCreep2.html) (obsoletes ICWMaterial::IncludeCreep)* [ICWMaterial::SetMaterialDataCurve3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetMaterialDataCurve3.html) (obsoletes ICWMaterial::SetMaterialDataCurve)

#### ICWMesh interface

* [ICWMesh::AutomaticLooping2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~AutomaticLooping2.html) (obsoletes ICWMesh::AutomaticLooping)* [ICWMesh::AutomaticTransition2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~AutomaticTransition2.html) (obsoletes ICWMesh::AutomaticTransition)* [ICWMesh::GetPoorMeshQualityElementList2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetPoorMeshQualityElementList2.html) (obsoletes ICWMesh::GetPoorMeshQualityElementList)* [ICWMesh::IsComponentFailed2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~IsComponentFailed2.html) (obsoletes ICWMesh::IsComponentFailed)* [ICWMesh::IsMeshFailed2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~IsMeshFailed2.html) (obsoletes ICWMesh::IsMeshFailed)* [ICWMesh::NegativeJacobianRatioCheck2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~NegativeJacobianRatioCheck2.html) (obsoletes ICWMesh::NegativeJacobianRatioCheck)* [ICWMesh::SaveSettingsWithoutMeshing2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~SaveSettingsWithoutMeshing2.html) (obsoletes ICWMesh::SaveSettingsWithoutMeshing)* [ICWMesh::SetMeshAndParamsForDefaultBCB](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~SetMeshAndParamsForDefaultBCB.html)* [ICWMesh::UseJacobianCheckForShells2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~UseJacobianCheckForShells2.html) (obsoletes ICWMesh::UseJacobianCheckForShells)

#### ICWMeshControl interface

* [ICWMeshControl::BeamSelected2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~BeamSelected2.html) (obsoletes ICWMeshControl::BeamSelected)* [ICWMeshControl::GetEntityAt3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~GetEntityAt3.html) (obsoletes ICWMeshControl::GetEntityAt2)* [ICWMeshControl::UseSameElementSize2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~UseSameElementSize2.html) (obsoletes ICWMeshControl::UseSameElementSize)

#### ICWMultipleComponentContactsEditManager interface

* [ICWMultipleComponentContactsEditManager::IncludeClearance2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~IncludeClearance2.html) (obsoletes ICWMultipleComponentContactsEditManager::IncludeClearance)* [ICWMultipleComponentContactsEditManager::IncludeShellEdgeSolidOrShellFace2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~IncludeShellEdgeSolidOrShellFace2.html) (obsoletes ICWMultipleComponentContactsEditManager::IncludeShellEdgeSolidOrShellFace)* [ICWMultipleComponentContactsEditManager::SetIncludeFriction2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~SetIncludeFriction2.html) (obsoletes ICWMultipleComponentContactsEditManager::SetIncludeFriction)

#### ICWPinConnector interface

* [ICWPinConnector::AllowDistributedCoupling2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector~AllowDistributedCoupling2.html) (obsoletes ICWPinConnector::AllowDistributedCoupling)

#### ICWPressure interface

* [ICWPressure::ReverseDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~ReverseDirection2.html) (obsoletes ICWPressure::ReverseDirection)* [ICWPressure::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetTimeCurve2.html) (obsoletes ICWPressure::SetTimeCurve)

#### ICWRadiation interface

* [ICWRadiation::OpenSystem2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation~OpenSystem2.html) (obsoletes ICWRadiation::OpenSystem)* [ICWRadiation::SetTemperatureCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation~SetTemperatureCurve2.html) (obsoletes ICWRadiation::SetTemperatureCurve)* [ICWRadiation::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation~SetTimeCurve2.html) (obsoletes ICWRadiation::SetTimeCurve)* [ICWRadiation::UseTemperatureCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation~UseTemperatureCurve2.html) (obsoletes ICWRadiation::UseTemperatureCurve)* [ICWRadiation::UseTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation~UseTimeCurve2.html) (obsoletes ICWRadiation::UseTimeCurve)

#### ICWRemoteLoad interface

* [ICWRemoteLoad::AllowDistributedCoupling2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~AllowDistributedCoupling2.html) (obsoletes ICWRemoteLoad::AllowDistributedCoupling)* [ICWRemoteLoad::GetForceOrTranslationValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetForceOrTranslationValues2.html) (obsoletes ICWRemoteLoad::GetForceOrTranslationValues)* [ICWRemoteLoad::GetMassValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetMassValues2.html) (obsoletes ICWRemoteLoad::GetMassValues)* [ICWRemoteLoad::GetMomentOrRotationValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetMomentOrRotationValues2.html) (obsoletes ICWRemoteLoad::GetMomentOrRotationValues)* [ICWRemoteLoad::SetForceOrTranslationValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetForceOrTranslationValues2.html) (obsoletes ICWRemoteLoad::SetForceOrTranslationValues)* [ICWRemoteLoad::SetForceOrTranslationValuesEx2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetForceOrTranslationValuesEx2.html) (obsoletes ICWRemoteLoad::SetForceOrTranslationValuesEx)* [ICWRemoteLoad::SetMassValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMassValues2.html) (obsoletes ICWRemoteLoad::SetMassValues)* [ICWRemoteLoad::SetMomentOrRotationValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValues2.html) (obsoletes ICWRemoteLoad::SetMomentOrRotationValues)* [ICWRemoteLoad::SetMomentOrRotationValuesEx2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValuesEx2.html) (obsoletes ICWRemoteLoad::SetMomentOrRotationValuesEx)* [ICWRemoteLoad::SetReferenceCoordinateSystem2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetReferenceCoordinateSystem2.html) (obsoletes ICWRemoteLoad::SetReferenceCoordinateSystem)* [ICWRemoteLoad::SetTimeOrFrequencyCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetTimeOrFrequencyCurve2.html) (obsoletes ICWRemoteLoad::SetTimeOrFrequencyCurve)

#### ICWResults interface

* [ICWResults::GetHeatPowerOrEnergy2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetHeatPowerOrEnergy2.html) (obsoletes ICWResults::GetHeatPowerOrEnergy)* [ICWResults::GetMinMaxFactorOfSafety2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafety2.html) (obsoletes ICWResults::GetMinMaxFactorOfSafety)* [ICWResults::GetMinMaxStressForHarmonic2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxStressForHarmonic2.html) (obsoletes ICWResults::GetMinMaxStressForHarmonic)

#### ICWShell interface

* [ICWShell::SetFavMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetFavMaterial2.html) (obsoletes ICWShell::SetFavMaterial)* [ICWShell::SetLibraryMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetLibraryMaterial2.html) (obsoletes ICWShell::SetLibraryMaterial)

#### ICWSolidBody interface

* [ICWSolidBody::SetFavMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody~SetFavMaterial2.html) (obsoletes ICWSolidBody::SetFavMaterial)* [ICWSolidBody::SetLibraryMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody~SetLibraryMaterial2.html) (obsoletes ICWSolidBody::SetLibraryMaterial)

#### ICWStudyManager interface

* [ICWStudyManager::ManageDistributedSimulation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~ManageDistributedSimulation2.html) (obsoletes ICWStudyManager::ManageDistributedSimulation)* [ICWStudyManager::SetDistributedSimulation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~SetDistributedSimulation2.html) (obsoletes ICWStudyManager::SetDistributedSimulation)

#### ICWStudyResultOptions interface

* [ICWStudyResultOptions::GetSaveStressAndReactionsOptions2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~GetSaveStressAndReactionsOptions2.html) (obsoletes ICWStudyResultOptions::GetSaveStressAndReactionsOptions)* [ICWStudyResultOptions::SaveReactions2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SaveReactions2.html) (obsoletes ICWStudyResultOptions::SaveReactions)* [ICWStudyResultOptions::SaveStresses2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SaveStresses2.html) (obsoletes ICWStudyResultOptions::SaveStresses)* [ICWStudyResultOptions::SetSaveStressAndReactionsOptions2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SetSaveStressAndReactionsOptions2.html) (obsoletes ICWStudyResultOptions::SetSaveStressAndReactionsOptions)

#### ICWTemperature interface

* [ICWTemperature::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTemperature~SetTimeCurve2.html) (obsoletes ICWTemperature::SetTimeCurve)* [ICWTemperature::UseTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTemperature~UseTimeCurve2.html) (obsoletes ICWTemperature::UseTimeCurve)

#### ICWThermalStudyOptions interface

* [ICWThermalStudyOptions::CheckFlowConvectionCoef2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWThermalStudyOptions~CheckFlowConvectionCoef2.html) (obsoletes ICWThermalStudyOptions::CheckFlowConvectionCoef)* [ICWThermalStudyOptions::Email2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWThermalStudyOptions~EMail2.html) (obsoletes ICWThermalStudyOptions::Email)* [ICWThermalStudyOptions::EmailTimebased2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWThermalStudyOptions~EMailTimebased2.html) (obsoletes ICWThermalStudyOptions::EmailTimebased)* [ICWThermalStudyOptions::UseTemperatureFromThermalStudy2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWThermalStudyOptions~UseTemperatureFromThermalStudy2.html) (obsoletes ICWThermalStudyOptions::UseTemperatuareFromThermalStudy)

#### ICWTopologyDemoldControl interface

* [ICWTopologyDemoldControl::SetAutoDetermineCentralMidPlane2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl~SetAutoDetermineCentralMidPlane2.html) (obsoletes ICWTopologyDemoldControl::SetAutoDetermineCentralMidPlane)* [ICWTopologyDemoldControl::SetReverseDirection2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl~SetReverseDirection2.html) (obsoletes ICWTopologyDemoldControl::SetReverseDirection)

#### ICWTopologyFrequencyConstraint interface

* [ICWTopologyFrequencyConstraint::SetModeTrackingFlag2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFrequencyConstraint~SetModeTrackingFlag2.html) (obsoletes ICWTopologyFrequencyConstraint::SetModeTrackingFlag)

#### ICWTopologyPreservedRegionControl interface

* [ICWTopologyPreservedRegionControl::SetIncludeRegionDepth2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyPreservedRegionControl~SetIncludeRegionDepth2.html) (obsoletes ICWTopologyPreservedRegionControl::SetIncludeRegionDepth)

#### ICWTopologyThicknessControl interface

* [ICWTopologyThicknessControl::SetIncludeMaxMemberThickness2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl~SetIncludeMaxMemberThickness2.html) (obsoletes ICWTopologyThicknessControl::SetIncludeMaxMemberThickness)* [ICWTopologyThicknessControl::SetIncludeMinMemberThickness2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl~SetIncludeMinMemberThickness2.html) (obsoletes ICWTopologyThicknessControl::SetIncludeMinMemberThickness)

#### [Back to top](#top)