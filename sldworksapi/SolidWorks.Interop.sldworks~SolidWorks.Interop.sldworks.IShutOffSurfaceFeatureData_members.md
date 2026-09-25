<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IShutOffSurfaceFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IShutOffSurfaceFeatureData Interface |

The following tables list the members exposed by [IShutOffSurfaceFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Edges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~Edges.html) | Gets or sets the edges that form closed loops for the patches. |
| ![ Property](dotnetimages/Property.gif) | [Knit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~Knit.html) | Gets or sets whether to knit the patches in this shut-off surface feature. |
| ![ Property](dotnetimages/Property.gif) | [LoopEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~LoopEdges.html) | Gets the edges in the specified loop in this shut-off surface feature. |
| ![ Property](dotnetimages/Property.gif) | [LoopPatchType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~LoopPatchType.html) | Gets and sets the type of patch for the specified loop for this shut-off surface feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~AccessSelections.html) | Gains access to the selections that define this shut-off surface feature. |
| ![ Method](dotnetimages/Method.gif) | [FlipFaceTangentTo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~FlipFaceTangentTo.html) | Indicates to create the patch on the opposite tangent face. |
| ![ Method](dotnetimages/Method.gif) | [GetEdgeCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~GetEdgeCount.html) | Gets the number of edges that form a closed loop. |
| ![ Method](dotnetimages/Method.gif) | [GetFaceTangentTo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~GetFaceTangentTo.html) | Gets the tangent face for the specified loop where to create the patch. |
| ![ Method](dotnetimages/Method.gif) | [GetLoopCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~GetLoopCount.html) | Gets the number of closed loops for all of the patches. |
| ![ Method](dotnetimages/Method.gif) | [GetLoopEdgeCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~GetLoopEdgeCount.html) | Gets the number of edges in the specified loop. |
| ![ Method](dotnetimages/Method.gif) | [IGetEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~IGetEdges.html) | Gets the edges that form closed loops to use for the patches. |
| ![ Method](dotnetimages/Method.gif) | [IGetLoopEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~IGetLoopEdges.html) | Gets the edges in the specified loop. |
| ![ Method](dotnetimages/Method.gif) | [ISetEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~ISetEdges.html) | Sets the edges to use to form closed loops for patches. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections that define this shut-off surface feature. |
| ![ Method](dotnetimages/Method.gif) | [SetAllPatchTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~SetAllPatchTypes.html) | Sets the type of patch for all loops for this shut-off surface feature. |
| ![ Method](dotnetimages/Method.gif) | [Status](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData~Status.html) | Gets the status of the shut-off surface feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IShutOffSurfaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::InsertMoldShutOffSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldShutOffSurface.html)