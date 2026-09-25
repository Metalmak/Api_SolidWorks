<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICosmeticWeldBeadFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ICosmeticWeldBeadFeatureData Interface |

The following tables list the members exposed by [ICosmeticWeldBeadFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [BeadSize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~BeadSize.html) | Gets or sets the thickness of a weld bead. |
| ![ Property](dotnetimages/Property.gif) | [FromToLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~FromToLength.html) | Gets or sets whether to enable the from/to length properties. |
| ![ Property](dotnetimages/Property.gif) | [FromToReverse](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~FromToReverse.html) | Gets or sets whether to start the weld from the opposite end. |
| ![ Property](dotnetimages/Property.gif) | [FromToStartPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~FromToStartPoint.html) | Gets or sets the position of the first weld bead with respect to the end of the selected face or edge. |
| ![ Property](dotnetimages/Property.gif) | [FromToWeldLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~FromToWeldLength.html) | Gets or sets the length of the weld. |
| ![ Property](dotnetimages/Property.gif) | [Gap](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~Gap.html) | Gets or sets the gap between intermittent weld beads. |
| ![ Property](dotnetimages/Property.gif) | [GapOrPitch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GapOrPitch.html) | Gets or sets whether to use gap or pitch spacing for intermittent weld beads. |
| ![ Property](dotnetimages/Property.gif) | [IntermittentWeld](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~IntermittentWeld.html) | Gets or sets whether to enable intermittent weld properties. |
| ![ Property](dotnetimages/Property.gif) | [IntermittentWeldLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~IntermittentWeldLength.html) | Gets or sets the length of the weld for intermittent weld beads. |
| ![ Property](dotnetimages/Property.gif) | [Pitch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~Pitch.html) | Gets or sets the pitch of intermittent weld beads. |
| ![ Property](dotnetimages/Property.gif) | [Side](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~Side.html) | Gets or sets how the weld bead is applied to selected faces or edges. |
| ![ Property](dotnetimages/Property.gif) | [Staggered](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~Staggered.html) | Gets or sets whether to alternate the positioning of the weld beads on both sides of the weld body. |
| ![ Property](dotnetimages/Property.gif) | [TangentPropagation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~TangentPropagation.html) | Gets or sets whether to apply the weld bead to all edges that are tangent to the selected faces or edges. |
| ![ Property](dotnetimages/Property.gif) | [WeldSymbol](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~WeldSymbol.html) | Gets or sets the weld symbol for this weld bead. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~AccessSelections.html) | Gains access to the selections that define this cosmetic weld bead feature. |
| ![ Method](dotnetimages/Method.gif) | [GetEntities](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GetEntities.html) | Obsolete. Superseded by [ICosmeticWeldBeadFeatureData::GetEntitiesWeldFrom](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GetEntitiesWeldFrom.html) and [ICosmeticWeldBeadFeatureData::GetEntitiesWeldTo.](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GetEntitiesWeldTo.html) |
| ![ Method](dotnetimages/Method.gif) | [GetEntitiesWeldFrom](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GetEntitiesWeldFrom.html) | Gets the weld-from entity type and weld-from entities for this cosmetic weld bead, which was created using weld geometry. |
| ![ Method](dotnetimages/Method.gif) | [GetEntitiesWeldPath](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GetEntitiesWeldPath.html) | Gets the entities for this cosmetic weld bead, which was created using a weld path. |
| ![ Method](dotnetimages/Method.gif) | [GetEntitiesWeldTo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GetEntitiesWeldTo.html) | Gets the weld-to entity type and weld-to entities for this cosmetic weld bead, which was created using weld geometry. |
| ![ Method](dotnetimages/Method.gif) | [GetReferenceEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GetReferenceEdges.html) | Gets the reference edges created by this cosmetic weld bead feature. |
| ![ Method](dotnetimages/Method.gif) | [GetWeldBeadFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~GetWeldBeadFolder.html) | Gets the weld bead folder. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections that define this cosmetic weld bead feature. |
| ![ Method](dotnetimages/Method.gif) | [SetEntities](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~SetEntities.html) | Obsolete. Superseded by [ICosmeticWeldBeadFeatureData::SetEntitiesWeldFrom](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~SetEntitiesWeldFrom.html) and [ICosmeticWeldBeadFeatureData::SetEntitiesWeldTo.](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~SetEntitiesWeldTo.html) |
| ![ Method](dotnetimages/Method.gif) | [SetEntitiesWeldFrom](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~SetEntitiesWeldFrom.html) | Sets the weld-from entities for this cosmetic weld bead, which was created using weld geometry. |
| ![ Method](dotnetimages/Method.gif) | [SetEntitiesWeldPath](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~SetEntitiesWeldPath.html) | Sets the entities for this cosmetic weld bead, which was created using a weld path. |
| ![ Method](dotnetimages/Method.gif) | [SetEntitiesWeldTo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData~SetEntitiesWeldTo.html) | Sets the weld-to entities for this cosmetic weld bead, which was created using weld geometry. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICosmeticWeldBeadFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ICosmeticWeldBeadFolder Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFolder.html)

[IFeatureManager::InsertCosmeticWeldBead2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertCosmeticWeldBead2.html)