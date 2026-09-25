<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IPartingLineFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IPartingLineFeatureData Interface |

The following tables list the members exposed by [IPartingLineFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Angle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~Angle.html) | Gets or sets the draft angle for the parting line. |
| ![ Property](dotnetimages/Property.gif) | [CoreCavitySplit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~CoreCavitySplit.html) | Gets or sets the core/cavity split option for a parting line. |
| ![ Property](dotnetimages/Property.gif) | [PartingLines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~PartingLines.html) | Gets and sets the edges for the parting lines. |
| ![ Property](dotnetimages/Property.gif) | [PullDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~PullDirection.html) | Gets whether the direction of pull is reversed. |
| ![ Property](dotnetimages/Property.gif) | [PullDirectionBase](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~PullDirectionBase.html) | Gets or sets the direction of pull for the parting line feature. |
| ![ Property](dotnetimages/Property.gif) | [PullDirectionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~PullDirectionType.html) | Gets the type of entity indicating the direction of pull. |
| ![ Property](dotnetimages/Property.gif) | [SplitFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~SplitFaces.html) | Gets or sets whether to split faces. |
| ![ Property](dotnetimages/Property.gif) | [SplitFacesOption](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~SplitFacesOption.html) | Gets or sets the split faces option for this parting line. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~AccessSelections.html) | Gains access to the selections that describe the parting line feature. |
| ![ Method](dotnetimages/Method.gif) | [DraftAnalysis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~DraftAnalysis.html) | Performs draft analysis for the input angle and the direction of pull. |
| ![ Method](dotnetimages/Method.gif) | [GetEntitiesToSplit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~GetEntitiesToSplit.html) | Gets the entities that are used to split a face. |
| ![ Method](dotnetimages/Method.gif) | [GetEntitiesToSplitCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~GetEntitiesToSplitCount.html) | Gets the number of entities to use to split a face and add edges to the parting line feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFacesByType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~GetFacesByType.html) | Gets the specified faces after performing a draft analysis of the parting line feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFacesByTypeCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~GetFacesByTypeCount.html) | Gets the number of faces of the specified type for this parting line. |
| ![ Method](dotnetimages/Method.gif) | [GetPartingLinesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~GetPartingLinesCount.html) | Gets the number of edges used as parting lines. |
| ![ Method](dotnetimages/Method.gif) | [IGetEntitiesToSplit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~IGetEntitiesToSplit.html) | Gets the entities that are used to split a face. |
| ![ Method](dotnetimages/Method.gif) | [IGetFacesByType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~IGetFacesByType.html) | Gets the specified faces after performing a draft analysis of the parting line feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetPartingLines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~IGetPartingLines.html) | Gets the edges used as parting lines. |
| ![ Method](dotnetimages/Method.gif) | [ISetEntitiesToSplit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~ISetEntitiesToSplit.html) | Sets the entities to use to split a face and add edges to the parting line feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetPartingLines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~ISetPartingLines.html) | Sets the edges to use as parting lines. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections that define this parting line feature. |
| ![ Method](dotnetimages/Method.gif) | [SetEntitiesToSplit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~SetEntitiesToSplit.html) | Sets the entities to use to split a face and add edges to the parting line feature. |
| ![ Method](dotnetimages/Method.gif) | [Status](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~Status.html) | Gets the status of this parting line feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IPartingLineFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::InsertMoldPartingLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldPartingLine.html)

[ICavityFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData.html)

[ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html)

[IPartingSurfaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingSurfaceFeatureData.html)

[IRuledSurfaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRuledSurfaceFeatureData.html)

[IShutOffSurfaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData.html)

[IToolingSplitFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IToolingSplitFeatureData.html)

[IMoveFaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData.html)