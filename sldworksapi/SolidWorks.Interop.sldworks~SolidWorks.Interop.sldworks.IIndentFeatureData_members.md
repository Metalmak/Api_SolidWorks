<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IIndentFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IIndentFeatureData Interface |

The following tables list the members exposed by [IIndentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Clearance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~Clearance.html) | Gets or sets the clearance between the target and tool bodies in this indent feature. |
| ![ Property](dotnetimages/Property.gif) | [ClearanceDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~ClearanceDirection.html) | Gets or sets the direction of the [clearance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~Clearance.html) for this indent feature. |
| ![ Property](dotnetimages/Property.gif) | [CutDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~CutDirection.html) | Gets or sets whether to flip the side of the cut for this indent feature. |
| ![ Property](dotnetimages/Property.gif) | [IsCut](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~IsCut.html) | Gets or sets whether to remove the intersection area of the [target body](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~TargetBody.html). |
| ![ Property](dotnetimages/Property.gif) | [SelectionState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~SelectionState.html) | Gets or sets the side of the model to keep or remove. |
| ![ Property](dotnetimages/Property.gif) | [TargetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~TargetBody.html) | Gets or sets the solid or surface body to indent. |
| ![ Property](dotnetimages/Property.gif) | [Thickness](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~Thickness.html) | Gets or sets the thickness of the indent feature. |
| ![ Property](dotnetimages/Property.gif) | [ToolBodyRegion](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~ToolBodyRegion.html) | Gets or sets the tool body region for the indent feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~AccessSelections.html) | Gains access to the selections that define this indent feature. |
| ![ Method](dotnetimages/Method.gif) | [GetBodiesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~GetBodiesCount.html) | Gets the number of solid or surface [bodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) for the [tool body region](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~ToolBodyRegion.html). |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections for this indent feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IIndentFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::InsertIndent Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertIndent.html)