<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMate2 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IMate2 Interface |

The following tables list the members exposed by [IMate2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Alignment](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~Alignment.html) | Gets the type of alignment for this mate. |
| ![ Property](dotnetimages/Property.gif) | [CanBeFlipped](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~CanBeFlipped.html) | Gets whether this distance or angle mate can be flipped. |
| ![ Property](dotnetimages/Property.gif) | [DisplayDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~DisplayDimension.html) | Obsolete. Superseded by [IMate2::DisplayDimension2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMate2~DisplayDimension2.html). |
| ![ Property](dotnetimages/Property.gif) | [DisplayDimension2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~DisplayDimension2.html) | Gets the specified display dimension for this mate. |
| ![ Property](dotnetimages/Property.gif) | [DistanceFirstArcCondition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~DistanceFirstArcCondition.html) | Gets the the first arc condition of this distance mate between cylindrical components. |
| ![ Property](dotnetimages/Property.gif) | [DistanceSecondArcCondition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~DistanceSecondArcCondition.html) | Gets the the second arc condition of this distance mate between cylindrical components. |
| ![ Property](dotnetimages/Property.gif) | [Flipped](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~Flipped.html) | Gets or sets whether to flip the distance or angle mate. |
| ![ Property](dotnetimages/Property.gif) | [HasLoadBearingFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~HasLoadBearingFaces.html) | Gets whether this mate has load bearing faces. |
| ![ Property](dotnetimages/Property.gif) | [HasTreatInterferenceAsShrinkFit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~HasTreatInterferenceAsShrinkFit.html) | Gets whether interference in this mate is treated as shrink/press fit. |
| ![ Property](dotnetimages/Property.gif) | [IsLoadBearingFacesBonded](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~IsLoadBearingFacesBonded.html) | Get whether the load bearing faces of this mate are bonded. |
| ![ Property](dotnetimages/Property.gif) | [LockMagneticMate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~LockMagneticMate.html) | Gets or sets whether to lock this magnetic mate. |
| ![ Property](dotnetimages/Property.gif) | [MateLoadReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~MateLoadReference.html) | Gets the mate load reference associated with this mate. |
| ![ Property](dotnetimages/Property.gif) | [MaximumVariation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~MaximumVariation.html) | Gets the maximum variation, in meters or radians, for the dimension of this distance or angle mate. |
| ![ Property](dotnetimages/Property.gif) | [MinimumVariation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~MinimumVariation.html) | Gets the minimum variation, in meters or radians, for the dimension of this distance or angle mate. |
| ![ Property](dotnetimages/Property.gif) | [Type](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~Type.html) | Gets the type of mate. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [ForceMisalignment](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~ForceMisalignment.html) | Forces a misaligned mate condition for this concentric mate. |
| ![ Method](dotnetimages/Method.gif) | [GetConcentricAlignmentType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetConcentricAlignmentType.html) | Gets the alignment type of this mate. |
| ![ Method](dotnetimages/Method.gif) | [GetCurrentMisalignedDeviation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetCurrentMisalignedDeviation.html) | Gets the current misalignment deviation for the misaligned concentric mate. |
| ![ Method](dotnetimages/Method.gif) | [GetForce](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetForce.html) | Gets the magnitude and direction of the force applied to this mate. |
| ![ Method](dotnetimages/Method.gif) | [GetLinkedMate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetLinkedMate.html) | Gets the linked mate of this concentric mate. |
| ![ Method](dotnetimages/Method.gif) | [GetMateEntityCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetMateEntityCount.html) | Gets the number of entities for this mate. |
| ![ Method](dotnetimages/Method.gif) | [GetMaximumMisalignedDeviation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetMaximumMisalignedDeviation.html) | Gets the maximum allowed misalignment deviation for this misaligned concentric mate. |
| ![ Method](dotnetimages/Method.gif) | [GetSupplementalFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetSupplementalFaces.html) | Gets the faces in this mate. |
| ![ Method](dotnetimages/Method.gif) | [GetTorque](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetTorque.html) | Gets the angle and the axis of the torque applied to this mate. |
| ![ Method](dotnetimages/Method.gif) | [GetUseMisalignedDeviationDocumentProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetUseMisalignedDeviationDocumentProperty.html) | Gets whether to use the document property value for the maximum misalignment deviation of the misaligned concentric mate. |
| ![ Method](dotnetimages/Method.gif) | [IGetSupplementalFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~IGetSupplementalFaces.html) | Gets the faces in this mate. |
| ![ Method](dotnetimages/Method.gif) | [MateEntity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~MateEntity.html) | Gets an entity associated with a mate. |
| ![ Method](dotnetimages/Method.gif) | [RemoveMisalignment](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~RemoveMisalignment.html) | Removes the misaligned mate condition of this concentric mate. |
| ![ Method](dotnetimages/Method.gif) | [SetConcentricAlignmentType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~SetConcentricAlignmentType.html) | Sets the alignment type of this mate. |
| ![ Method](dotnetimages/Method.gif) | [SetForce](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~SetForce.html) | Sets the magnitude and direction of the force to apply to this mate. |
| ![ Method](dotnetimages/Method.gif) | [SetMaximumMisalignedDeviation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~SetMaximumMisalignedDeviation.html) | Sets the maximum allowed misalignment deviation for this misaligned concentric mate. |
| ![ Method](dotnetimages/Method.gif) | [SetTorque](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~SetTorque.html) | Sets the angle and the axis of the torque to apply to this mate. |
| ![ Method](dotnetimages/Method.gif) | [SetUseMisalignedDeviationDocumentProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~SetUseMisalignedDeviationDocumentProperty.html) | Sets whether to use the document property value for the maximum misalignment deviation for the misaligned concentric mate. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IMate2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IMateEntity2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateEntity2.html)

[IMateLoadReference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateLoadReference.html)

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)