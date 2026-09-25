<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWBeamBody Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWBeamBody Interface |

The following tables list the members exposed by [ICWBeamBody](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [BeamBodyName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamBodyName.html) | Gets the name of the beam. |
| ![ Property](dotnetimages/Property.gif) | [BeamDistForMaxShearStress](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamDistForMaxShearStress.html) | Gets or sets the maximum distance from the shear center to the furthest point on the cross-section of this beam body. |
| ![ Property](dotnetimages/Property.gif) | [BeamEnd1ConnectionType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamEnd1ConnectionType.html) | Gets or sets the End1 connection for this beam. |
| ![ Property](dotnetimages/Property.gif) | [BeamEnd2ConnectionType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamEnd2ConnectionType.html) | Gets or sets the End2 connection for this beam. |
| ![ Property](dotnetimages/Property.gif) | [BeamShearY](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamShearY.html) | Gets or sets the shear factor in direction 1 of the cross-section of this beam body. |
| ![ Property](dotnetimages/Property.gif) | [BeamShearZ](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamShearZ.html) | Gets or sets the shear factor in direction 2 of the cross-section of this beam body. |
| ![ Property](dotnetimages/Property.gif) | [BeamTorsionalConstant](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamTorsionalConstant.html) | Gets or sets the torsional stiffness constant for the cross-section of this beam body. |
| ![ Property](dotnetimages/Property.gif) | [BeamTorsionalConstantUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamTorsionalConstantUnit.html) | Gets or sets the units of length for cross-section calculations of this beam body. |
| ![ Property](dotnetimages/Property.gif) | [BeamType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamType.html) | Gets or sets the type of beam. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [BeamBeginEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamBeginEdit.html) | Begins editing of a beam. |
| ![ Method](dotnetimages/Method.gif) | [BeamEndEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamEndEdit.html) | Ends editing of a beam. |
| ![ Method](dotnetimages/Method.gif) | [ConvertToSolidBody](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~ConvertToSolidBody.html) | Treats a beam as a solid body. |
| ![ Method](dotnetimages/Method.gif) | [GetBeamBodyMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetBeamBodyMaterial.html) | Gets the material applied to the beam for analysis. |
| ![ Method](dotnetimages/Method.gif) | [GetDefaultMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetDefaultMaterial.html) | Gets the CAD material of the beam. |
| ![ Method](dotnetimages/Method.gif) | [GetManualEnd1ConnectionType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd1ConnectionType.html) | Obsolete. Superseded by [ICWBeamBody::GetManualEnd1ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd1ConnectionType2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetManualEnd1ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd1ConnectionType2.html) | Gets whether manual forces and moments are known to be zero for the End1 connection of the beam. |
| ![ Method](dotnetimages/Method.gif) | [GetManualEnd2ConnectionType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd2ConnectionType.html) | Obsolete. Superseded by [ICWBeamBody::GetManualEnd2ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd2ConnectionType2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetManualEnd2ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd2ConnectionType2.html) | Gets whether manual forces and moments are known to be zero for End2 connection of the beam. |
| ![ Method](dotnetimages/Method.gif) | [SetBeamBodyMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetBeamBodyMaterial.html) | Sets the material for the beam for analysis. |
| ![ Method](dotnetimages/Method.gif) | [SetFavMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetFavMaterial.html) | Obsolete. Superseded by [ICWBeamBody::SetFavMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetFavMaterial2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetFavMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetFavMaterial2.html) | Applies the specified material from the material favorites list. |
| ![ Method](dotnetimages/Method.gif) | [SetLibraryMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetLibraryMaterial.html) | Obsolete. Superseded by [ICWBeamBody::SetLibraryMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetLibraryMaterial2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetLibraryMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetLibraryMaterial2.html) | Sets the material library and material name for the beam. |
| ![ Method](dotnetimages/Method.gif) | [SetManualEnd1ConnectionType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd1ConnectionType.html) | Obsolete. Superseded by [ICWBeamBody::SetManualEnd1ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd1ConnectionType2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetManualEnd1ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd1ConnectionType2.html) | Sets whether manual forces and moments are known to be zero for End1 connection of the beam. |
| ![ Method](dotnetimages/Method.gif) | [SetManualEnd2ConnectionType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd2ConnectionType.html) | Obsolete. Superseded by [ICWBeamBody::SetManualEnd2ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd2ConnectionType2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetManualEnd2ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd2ConnectionType2.html) | Sets whether manual forces and moments are known to be zero for End2 connection of the beam. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBeamBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWJoints Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints.html)