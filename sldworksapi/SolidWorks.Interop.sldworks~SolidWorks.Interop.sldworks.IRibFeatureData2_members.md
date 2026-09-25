<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IRibFeatureData2 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IRibFeatureData2 Interface |

The following tables list the members exposed by [IRibFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Body](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~Body.html) | Gets or sets the body where the rib is created. |
| ![ Property](dotnetimages/Property.gif) | [DraftAngle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~DraftAngle.html) | Gets or sets the draft angle for the rib. |
| ![ Property](dotnetimages/Property.gif) | [DraftFromWall](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~DraftFromWall.html) | Gets or sets whether to draft the rib from the wall interface or the sketch plane. |
| ![ Property](dotnetimages/Property.gif) | [DraftOutward](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~DraftOutward.html) | Gets or sets whether the rib has an outward draft. |
| ![ Property](dotnetimages/Property.gif) | [EnableDraft](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~EnableDraft.html) | Gets or sets whether the rib has an associated draft. |
| ![ Property](dotnetimages/Property.gif) | [ExtrusionDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~ExtrusionDirection.html) | Gets or sets the direction in which to extrude the rib. |
| ![ Property](dotnetimages/Property.gif) | [FlipSide](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~FlipSide.html) | Gets or sets whether material is added to the reverse side of the rib. |
| ![ Property](dotnetimages/Property.gif) | [IsTwoSided](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~IsTwoSided.html) | Gets or sets whether the rib is created on two sides of the midplane or in a single direction (see [IRibFeatureData2::ReverseThicknessDir](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRibFeatureData2~ReverseThicknessDir.html)). |
| ![ Property](dotnetimages/Property.gif) | [RefSketchIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~RefSketchIndex.html) | Gets or sets which sketch segment defines the draft direction of the rib feature. |
| ![ Property](dotnetimages/Property.gif) | [ReverseThicknessDir](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~ReverseThicknessDir.html) | Gets or sets whether the extrusion is on the reverse side of this single-sided rib. |
| ![ Property](dotnetimages/Property.gif) | [Thickness](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~Thickness.html) | Gets or set the overall thickness of the rib. |
| ![ Property](dotnetimages/Property.gif) | [Type](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~Type.html) | Gets or sets the type of rib. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~AccessSelections.html) | Gains access to the the selections for this rib feature. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~IAccessSelections.html) | Gains access to the the selections for this rib feature. |
| ![ Method](dotnetimages/Method.gif) | [NextReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~NextReference.html) | Cycles through the possible sketch entities that can be used to define the draft, if it is used, for ribs with multiple contours. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2~ReleaseSelectionAccess.html) | Releases access to the selections that define this rib feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IRibFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::InsertRib Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertRib.html)