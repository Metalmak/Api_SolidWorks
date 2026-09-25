<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISketch Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISketch Interface |

The following tables list the members exposed by [ISketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [IModelToSketchXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IModelToSketchXform.html) | Obsolete. Superseded by [ISketch::ModelToSketchTransform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~ModelToSketchTransform.html).  **NOTE:** **This property is a get-only property.** **Set is not implemented**. |
| ![ Property](dotnetimages/Property.gif) | [ModelToSketchTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~ModelToSketchTransform.html) | Gets the model-to-sketch transform for this sketch.  **NOTE:** **This property is a get-only property.** **Set is not implemented**. |
| ![ Property](dotnetimages/Property.gif) | [ModelToSketchXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~ModelToSketchXform.html) | Obsolete. Superseded by [ISketch::ModelToSketchTransform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~ModelToSketchTransform.html).  **NOTE:** **This property is a get-only property.** **Set is not implemented**. |
| ![ Property](dotnetimages/Property.gif) | [RelationManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~RelationManager.html) | Gets the sketch relation manager.  **NOTE:** **This property is a get-only property.** **Set is not implemented**. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AutoDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~AutoDimension.html) | Obsolete. Superseded by [ISketch::AutoDimension2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~AutoDimension2.html). |
| ![ Method](dotnetimages/Method.gif) | [AutoDimension2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~AutoDimension2.html) | Obsolete. Superseded by [ISketchManager::FullyDefineSketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~FullyDefineSketch.html). |
| ![ Method](dotnetimages/Method.gif) | [CheckFeatureUse](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~CheckFeatureUse.html) | Checks to see if this sketch is valid for use in creating a specified feature. |
| ![ Method](dotnetimages/Method.gif) | [ConstrainAll](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~ConstrainAll.html) | Attempts to solve all of the apparent relations in the sketch and returns the number of constraints that were added to the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetArcCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetArcCount.html) | Gets the number of arcs in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetArcs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetArcs.html) | Obsolete. Superseded by [ISketch::GetArcs2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetArcs2.html) and [ISketch::IGetArcs2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetArcs2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetArcs2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetArcs2.html) | Gets all of the arcs in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetAutomaticSolve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetAutomaticSolve.html) | Checks whether the computation to solve the sketch geometry of the part as modifications are automatically performed. |
| ![ Method](dotnetimages/Method.gif) | [GetConstrainedStatus](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetConstrainedStatus.html) | Gets the current constrained status of the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetContourEdgeCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetContourEdgeCount.html) | Gets the number of edges for this sketch contour. |
| ![ Method](dotnetimages/Method.gif) | [GetContourEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetContourEdges.html) | Gets the edges for a sketch that has one contour. |
| ![ Method](dotnetimages/Method.gif) | [GetDetachSegmentOnDrag](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetDetachSegmentOnDrag.html) | Gets the Detach Segment on Drag setting. |
| ![ Method](dotnetimages/Method.gif) | [GetEllipseCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetEllipseCount.html) | Gets the number of ellipses in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetEllipses](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetEllipses.html) | Obsolete. Superseded by [ISketch::GetEllipses3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetEllipses3.html) and [ISketch::IGetEllipses3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetEllipses3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetEllipses2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetEllipses2.html) | Obsolete. Superseded by [ISketch::GetEllipses3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetEllipses3.html) and [ISketch::IGetEllipses3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetEllipses3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetEllipses3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetEllipses3.html) | Gets all of the ellipses in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetLineCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetLineCount.html) | Obsolete. Superseded by [ISketch::GetLineCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetLineCount2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetLineCount2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetLineCount2.html) | Gets the number of lines in the sketch with an option to exclude or include crosshatch lines. |
| ![ Method](dotnetimages/Method.gif) | [GetLines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetLines.html) | Obsolete. Superseded by [ISketch::GetLines2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetLines2.html) and [ISketch::IGetLines2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetLines2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetLines2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetLines2.html) | Gets all of the lines in the sketch with an option to include or exclude crosshatch lines. |
| ![ Method](dotnetimages/Method.gif) | [GetParabolaCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetParabolaCount.html) | Gets the number of parabolas in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetParabolas](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetParabolas.html) | Obsolete. Superseded by [ISketch::GetParabolas2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetParabolas2.html) and [ISketch::IGetParabolas2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetParabolas2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetParabolas2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetParabolas2.html) | Gets all of the parabolas in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetPolyLineCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetPolyLineCount.html) | Not implemented. |
| ![ Method](dotnetimages/Method.gif) | [GetPolylines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetPolylines.html) | Not implemented. |
| ![ Method](dotnetimages/Method.gif) | [GetReferenceEntity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetReferenceEntity.html) | Gets the entity on which this sketch was created. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchBlockInstanceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchBlockInstanceCount.html) | Gets the number of block instances in this sketch (i.e., the sketch under which the block instances are displayed in the FeatureManager design tree). |
| ![ Method](dotnetimages/Method.gif) | [GetSketchBlockInstances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchBlockInstances.html) | Gets the block instances in this sketch (i.e., the sketch under which the block instances are displayed in the FeatureManager design tree). |
| ![ Method](dotnetimages/Method.gif) | [GetSketchContourCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchContourCount.html) | Gets the number of sketch contours in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchContours](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchContours.html) | Gets the sketch contours in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchHatches](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchHatches.html) | Gets an array of sketch hatches that exist in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPathCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchPathCount.html) | Gets the number of sketch paths in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPaths](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchPaths.html) | Gets the sketch paths in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPictureCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchPictureCount.html) | Gets the number of pictures on this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPictures](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchPictures.html) | Gets the pictures on this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchPoints.html) | Obsolete. Superseded by [ISketch::GetSketchPoints2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSketchPoints2.html), [ISketch::IGetSketchPoints2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetSketchPoints2.html), and [ISketch::IEnumSketchPoints](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IEnumSketchPoints.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPoints2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchPoints2.html) | Gets the sketch points in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPointsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchPointsCount.html) | Obsolete. Superseded by [ISketch::GetSketchPointsCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSketchPointsCount2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPointsCount2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchPointsCount2.html) | Gets the number of sketch points in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchRegionCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchRegionCount.html) | Gets the number of sketch regions in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchRegions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchRegions.html) | Gets the sketch regions in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchSegments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchSegments.html) | Gets the sketch segments in this sketch, which include line, arc, spline, parabola, and ellipse entities. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchSlotCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchSlotCount.html) | Gets the number of sketch slots in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchSlots](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchSlots.html) | Gets the sketch slots in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchTextSegments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchTextSegments.html) | Gets the sketch segments that represent the selected text in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSplineCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineCount.html) | Gets the number of splines in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSplineInterpolateCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineInterpolateCount.html) | Gets the number of points in the spline and number of splines in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSplineParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParams.html) | Obsolete. Superseded by [ISketch::GetSplineParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplineParams2.html) and [ISketch::IGetSplineParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetSplineParams2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSplineParams2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParams2.html) | Obsolete. Superseded by [ISketch::GetSplineParams3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplineParams3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSplineParams3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParams3.html) | Obsolete. Superseded by [ISketch::GetSplineParams4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplineParams4.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSplineParams4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParams4.html) | Obsolete. Superseded by [ISketch::GetSplineParams5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParams5.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSplineParams5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParams5.html) | Gets the parameterization data of the specified spline in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetSplineParamsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParamsCount.html) | Obsolete. Superseded by [ISketch::GetSplineParamsCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplineParamsCount2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSplineParamsCount2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParamsCount2.html) | Obsolete. Superseded by [ISketch::GetSplineParamsCount3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplineParamsCount3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSplineParamsCount3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParamsCount3.html) | Gets the number of splines in the sketch and the size of array required to hold the data for them. |
| ![ Method](dotnetimages/Method.gif) | [GetSplines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplines.html) | Gets information for each spline by tessellation instead of by interpolation as is done by [ISketch::GetSplinesInterpolate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplinesInterpolate.html) and [ISketch::IGetSplinesInterpolate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetSplinesInterpolate.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSplinesInterpolate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplinesInterpolate.html) | Gets the spline points by interpolation instead of by tessellation as is done by [ISketch::GetSplines](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplines.html) and [ISketch::IGetSplines](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetSplines.html). |
| ![ Method](dotnetimages/Method.gif) | [GetUserPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetUserPoints.html) | Obsolete. Superseded by [ISketch::GetUserPoints2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetUserPoints2.html) and [ISketch::IGetUserPoints2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetUserPoints2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetUserPoints2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetUserPoints2.html) | Gets all of the user points in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetUserPointsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetUserPointsCount.html) | Gets the number of user points in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [IEnumSketchHatches](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IEnumSketchHatches.html) | Gets the sketch hatches enumeration in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IEnumSketchPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IEnumSketchPoints.html) | Gets the sketch points enumeration in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IEnumSketchSegments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IEnumSketchSegments.html) | Gets the sketch segments enumeration in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IEnumSketchTextSegments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IEnumSketchTextSegments.html) | Gets the sketch segments enumeration for the selected text in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetArcs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetArcs.html) | Obsolete. Superseded by [ISketch::GetArcs2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetArcs2.html) and [ISketch::IGetArcs2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetArcs2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetArcs2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetArcs2.html) | Gets all of the arcs in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetContourEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetContourEdges.html) | Gets the edges for a sketch that has one contour. |
| ![ Method](dotnetimages/Method.gif) | [IGetEllipses](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetEllipses.html) | Obsolete. Superseded by [ISketch::GetEllipses3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetEllipses3.html) and [ISketch::IGetEllipses3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetEllipses3.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetEllipses2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetEllipses2.html) | Obsolete. Superseded by [ISketch::GetEllipses3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetEllipses3.html) and [ISketch::IGetEllipses3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetEllipses3.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetEllipses3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetEllipses3.html) | Gets all of the ellipses in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetLines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetLines.html) | Obsolete. Superseded by [ISketch::GetLines2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetLines2.html) and [ISketch::IGetLines2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetLines2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetLines2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetLines2.html) | Gets all of the lines in the sketch with an option to include or exclude crosshatch lines. |
| ![ Method](dotnetimages/Method.gif) | [IGetParabolas](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetParabolas.html) | Obsolete. Superseded by [ISketch::GetParabolas2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetParabolas2.html) and [ISketch::IGetParabolas2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetParabolas2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetParabolas2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetParabolas2.html) | Gets all of the parabolas in the sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetPolylines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetPolylines.html) | Not implemented. |
| ![ Method](dotnetimages/Method.gif) | [IGetSketchBlockInstances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSketchBlockInstances.html) | Gets the block instances in this sketch (i.e., the sketch under which the block instances are displayed in the FeatureManager design tree). |
| ![ Method](dotnetimages/Method.gif) | [IGetSketchContours](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSketchContours.html) | Gets the sketch contours in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetSketchPaths](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSketchPaths.html) | Gets the sketch paths in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetSketchPictures](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSketchPictures.html) | Gets the pictures on this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetSketchPoints2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSketchPoints2.html) | Gets the sketch points in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetSketchRegions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSketchRegions.html) | Gets the sketch regions in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetSketchSlots](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSketchSlots.html) | Gets the sketch slots in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [IGetSplineParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSplineParams.html) | Obsolete. Superseded by [ISketch::GetSplineParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplineParams2.html) and [ISketch::IGetSplineParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetSplineParams2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetSplineParams2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSplineParams2.html) | Obsolete. Superseded by [ISketch::IGetSplineParameters3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetSplineParams3.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetSplineParams3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSplineParams3.html) | Obsolete. Superseded by [ISketch::GetSplineParams4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSplineParams4.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetSplines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSplines.html) | Gets information for each spline by tessellation instead of by interpolation as is done by [ISketch::GetSplinesInterpolate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplinesInterpolate.html) and [ISketch::IGetSplinesInterpolate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetSplinesInterpolate.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetSplinesInterpolate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetSplinesInterpolate.html) | Gets the spline points by interpolation instead of by tessellation as is done by [ISketch::GetSplines](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetSplines.html) and [ISketch::IGetSplines](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetSplines.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetUserPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetUserPoints.html) | Obsolete. Superseded by [ISketch::GetUserPoints2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetUserPoints2.html) and [ISketch::IGetUserPoints2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~IGetUserPoints2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetUserPoints2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IGetUserPoints2.html) | Gets all of the user points in this sketch. |
| ![ Method](dotnetimages/Method.gif) | [InsertRouteLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~InsertRouteLine.html) | Inserts a route line in an explode line sketch or a 3D sketch to indicate component relationships. |
| ![ Method](dotnetimages/Method.gif) | [Is3D](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~Is3D.html) | Gets whether this sketch is 2D or 3D. |
| ![ Method](dotnetimages/Method.gif) | [IsBoundaryBoxSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IsBoundaryBoxSketch.html) | Determines whether the sketch is a boundary box. |
| ![ Method](dotnetimages/Method.gif) | [IsDerived](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IsDerived.html) | Gets whether a sketch is derived. |
| ![ Method](dotnetimages/Method.gif) | [IsShared](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IsShared.html) | Gets whether this sketch is used by more than one feature. |
| ![ Method](dotnetimages/Method.gif) | [IsSketchEditable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~IsSketchEditable.html) | Gets whether this sketch is editable. |
| ![ Method](dotnetimages/Method.gif) | [MergePoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~MergePoints.html) | Merges sketch points within a specified distance. |
| ![ Method](dotnetimages/Method.gif) | [SetAutomaticSolve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~SetAutomaticSolve.html) | Controls whether the computation to solve the sketch geometry of the part as modifications are automatically performed. |
| ![ Method](dotnetimages/Method.gif) | [SetDetachSegmentOnDrag](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~SetDetachSegmentOnDrag.html) | Sets the Detach Segment on Drag setting. |
| ![ Method](dotnetimages/Method.gif) | [SetSketchEditable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~SetSketchEditable.html) | Sets whether this sketch is editable. |
| ![ Method](dotnetimages/Method.gif) | [SetWorkingPlaneOrientation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~SetWorkingPlaneOrientation.html) | Sets the orientation for sketching geometry in a 3D sketch. It sets the planar location for new 2D and 3D geometry in a 3D sketch. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ISketchArc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchArc.html)

[ISketchBlockDefinition Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockDefinition.html)

[ISketchBlockInstance Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance.html)

[ISketchContour Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchContour.html)

[ISketchedBendFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchedBendFeatureData.html)

[ISketchEllipse Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchEllipse.html)

[ISketchHatch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchHatch.html)

[ISketchLine Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine.html)

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchParabola Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchParabola.html)

[ISketchPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData.html)

[ISketchPoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html)

[ISketchRegion Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRegion.html)

[ISketchRelation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelation.html)

[ISketchRelationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager.html)

[ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html)

[ISketchSpline Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline.html)

[ISketchText Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchText.html)