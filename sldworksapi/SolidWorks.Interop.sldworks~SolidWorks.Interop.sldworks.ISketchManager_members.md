<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISketchManager Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISketchManager Interface |

The following tables list the members exposed by [ISketchManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [ActiveSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~ActiveSketch.html) | Gets the active sketch. |
| ![ Property](dotnetimages/Property.gif) | [AddToDB](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddToDB.html) | Gets or sets whether sketch entities are added directly to the SOLIDWORKS database. |
| ![ Property](dotnetimages/Property.gif) | [AutoInference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AutoInference.html) | Obsolete. Superseded by [ISldWorks::GetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetUserPreferenceToggle.html) or [ISldWorks::SetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetUserPreferenceToggle.html) and swUserPreferenceToggle\_e.swSketchInference. |
| ![ Property](dotnetimages/Property.gif) | [AutoSolve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AutoSolve.html) | Gets or sets whether SOLIDWORKS automatically solves the sketch geometry of the part while creating it. |
| ![ Property](dotnetimages/Property.gif) | [CurvatureDensity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CurvatureDensity.html) | Gets or sets the scaling factor by which to adjust the density of the curvature combs for this spline. |
| ![ Property](dotnetimages/Property.gif) | [CurvatureScale](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CurvatureScale.html) | Gets or sets the scaling factor by which to adjust the size of the curvature combs for this spline. |
| ![ Property](dotnetimages/Property.gif) | [DisplayWhenAdded](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~DisplayWhenAdded.html) | Gets or sets whether new sketch entities are immediately displayed when created. |
| ![ Property](dotnetimages/Property.gif) | [Document](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~Document.html) | Gets the document for this [ISketchManager](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager.html) object. |
| ![ Property](dotnetimages/Property.gif) | [InferenceMode](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InferenceMode.html) | Obsolete. Superseded by [ISldWorks::GetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetUserPreferenceToggle.html) or [ISldWorks::SetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetUserPreferenceToggle.html) and swUserPreferenceToggle\_e.swSketchInference. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddAlongXDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddAlongXDimension.html) | Projects and displays along the x axis a dimension between selected points in a 3D sketch. |
| ![ Method](dotnetimages/Method.gif) | [AddAlongYDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddAlongYDimension.html) | Projects and displays along the y axis a dimension between selected points in a 3D sketch. |
| ![ Method](dotnetimages/Method.gif) | [AddAlongZDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddAlongZDimension.html) | Projects and displays along the z axis a dimension between selected points in a 3D sketch. |
| ![ Method](dotnetimages/Method.gif) | [ConvertEntities](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~ConvertEntities.html) | Not implemented. Use [ISketchManager::SketchUseEdge2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~SketchUseEdge2.html). |
| ![ Method](dotnetimages/Method.gif) | [Create3PointArc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~Create3PointArc.html) | Creates a 3-point arc. |
| ![ Method](dotnetimages/Method.gif) | [Create3PointCenterRectangle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~Create3PointCenterRectangle.html) | Creates a 3-point center rectangle at any angle. |
| ![ Method](dotnetimages/Method.gif) | [Create3PointCornerRectangle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~Create3PointCornerRectangle.html) | Creates a 3-point corner rectangle at any angle. |
| ![ Method](dotnetimages/Method.gif) | [CreateArc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateArc.html) | Creates an arc based on a center point, a start point, an end point, and a direction. |
| ![ Method](dotnetimages/Method.gif) | [CreateBoundaryHatch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateBoundaryHatch.html) | Creates area hatch/fill boundary hatches using closed sketch profiles. |
| ![ Method](dotnetimages/Method.gif) | [CreateCenterLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateCenterLine.html) | Creates a center line between the specified points. |
| ![ Method](dotnetimages/Method.gif) | [CreateCenterRectangle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateCenterRectangle.html) | Creates a center rectangle. |
| ![ Method](dotnetimages/Method.gif) | [CreateChamfer](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateChamfer.html) | Creates a chamfer between two selected sketch entities. |
| ![ Method](dotnetimages/Method.gif) | [CreateCircle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateCircle.html) | Creates a circle based on a center point and a point on the circle. |
| ![ Method](dotnetimages/Method.gif) | [CreateCircleByRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateCircleByRadius.html) | Creates a circle based on a center point and a specified radius. |
| ![ Method](dotnetimages/Method.gif) | [CreateCircularSketchStepAndRepeat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateCircularSketchStepAndRepeat.html) | Creates circular sketch pattern. |
| ![ Method](dotnetimages/Method.gif) | [CreateConic](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateConic.html) | Creates a conic curve in the active sketch. |
| ![ Method](dotnetimages/Method.gif) | [CreateConstructionGeometry](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateConstructionGeometry.html) | Sets selected sketch segments to be construction geometry instead of sketch geometry. |
| ![ Method](dotnetimages/Method.gif) | [CreateCornerRectangle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateCornerRectangle.html) | Creates a corner rectangle. |
| ![ Method](dotnetimages/Method.gif) | [CreateEllipse](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateEllipse.html) | Creates an ellipse using the specified center, major-axis, and minor-axis points. |
| ![ Method](dotnetimages/Method.gif) | [CreateEllipticalArc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateEllipticalArc.html) | Creates a partial ellipse given a center point, two points that specify the major and minor axis, and two points that define the elliptical start and end points. |
| ![ Method](dotnetimages/Method.gif) | [CreateEquationSpline](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateEquationSpline.html) | Obsolete. Superseded by [ISketchManager::CreateEquationSpline2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateEquationSpline2.html). |
| ![ Method](dotnetimages/Method.gif) | [CreateEquationSpline2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateEquationSpline2.html) | Creates an equation-driven 2D explicit or parametric curve or a 3D parametric curve. |
| ![ Method](dotnetimages/Method.gif) | [CreateFillet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateFillet.html) | Creates a sketch fillet using the selected sketch entities. |
| ![ Method](dotnetimages/Method.gif) | [CreateLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateLine.html) | Creates a sketch line in the currently active 2D or 3D sketch. |
| ![ Method](dotnetimages/Method.gif) | [CreateLinearSketchStepAndRepeat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateLinearSketchStepAndRepeat.html) | Creates a linear sketch pattern. |
| ![ Method](dotnetimages/Method.gif) | [CreateParabola](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateParabola.html) | Creates a parabola in the active sketch. |
| ![ Method](dotnetimages/Method.gif) | [CreateParallelogram](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateParallelogram.html) | Creates a parallelogram. |
| ![ Method](dotnetimages/Method.gif) | [CreatePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreatePoint.html) | Creates a sketch point in the active 2D or 3D sketch. |
| ![ Method](dotnetimages/Method.gif) | [CreatePolygon](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreatePolygon.html) | Creates a polygon in the active sketch. |
| ![ Method](dotnetimages/Method.gif) | [CreateRegionHatch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateRegionHatch.html) | Creates an area hatch/fill region hatch using a closed sketch profile. |
| ![ Method](dotnetimages/Method.gif) | [CreateSketchBelt](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSketchBelt.html) | Creates a sketch belt feature. |
| ![ Method](dotnetimages/Method.gif) | [CreateSketchPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSketchPlane.html) | Creates a 3D sketch plane. |
| ![ Method](dotnetimages/Method.gif) | [CreateSketchSlot](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSketchSlot.html) | Creates a sketch slot. |
| ![ Method](dotnetimages/Method.gif) | [CreateSpline](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSpline.html) | Obsolete. Superseded by [ISketchManager::CreateSpline2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateSpline2.html). |
| ![ Method](dotnetimages/Method.gif) | [CreateSpline2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSpline2.html) | Obsolete. Superseded by [ISketchManager::CreateSpline3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSpline3.html). |
| ![ Method](dotnetimages/Method.gif) | [CreateSpline3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSpline3.html) | Creates either a 2D spline or a spline constrained to a surface. |
| ![ Method](dotnetimages/Method.gif) | [CreateSplineByEqnParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSplineByEqnParams.html) | Creates a B-curve from B-spline data; that is, a set of B-spline vertices (control points) and a knot vector. |
| ![ Method](dotnetimages/Method.gif) | [CreateSplineParamData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSplineParamData.html) | Creates an empty spline parameter data object. |
| ![ Method](dotnetimages/Method.gif) | [CreateSplinesByEqnParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSplinesByEqnParams.html) | Obsolete. Superseded by [ISketchManager::CreateSplinesByEqnParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateSplinesByEqnParams2.html). |
| ![ Method](dotnetimages/Method.gif) | [CreateSplinesByEqnParams2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSplinesByEqnParams2.html) | Creates one or more spline segments using the B-curve parameters provided. |
| ![ Method](dotnetimages/Method.gif) | [CreateTangentArc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateTangentArc.html) | Creates a tangent arc. |
| ![ Method](dotnetimages/Method.gif) | [EditCircularSketchStepAndRepeat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~EditCircularSketchStepAndRepeat.html) | Edits a circular sketch pattern. |
| ![ Method](dotnetimages/Method.gif) | [EditLinearSketchStepAndRepeat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~EditLinearSketchStepAndRepeat.html) | Edits a linear sketch pattern. |
| ![ Method](dotnetimages/Method.gif) | [EditSketchBlock](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~EditSketchBlock.html) | Puts the block definition in edit mode. |
| ![ Method](dotnetimages/Method.gif) | [EndEditSketchBlock](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~EndEditSketchBlock.html) | Saves or discards your edits of the block and then ends the current editing session of this block. |
| ![ Method](dotnetimages/Method.gif) | [ExplodeSketchBlockInstance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~ExplodeSketchBlockInstance.html) | Explodes the specified block instance. |
| ![ Method](dotnetimages/Method.gif) | [FullyDefineSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~FullyDefineSketch.html) | Fully defines a sketch. |
| ![ Method](dotnetimages/Method.gif) | [GetDynamicMirror](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~GetDynamicMirror.html) | Gets whether dynamic sketch mirroring, which is the automatic mirroring of newly created sketch entities about a selected centerline, is enabled. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchBlockDefinitionCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~GetSketchBlockDefinitionCount.html) | Gets the number of block definitions in the model. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchBlockDefinitions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~GetSketchBlockDefinitions.html) | Gets all of the block definitions. |
| ![ Method](dotnetimages/Method.gif) | [ICreateSpline](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~ICreateSpline.html) | Obsolete. Superseded by [ISketchManager::ICreateSpline2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~ICreateSpline2.html). |
| ![ Method](dotnetimages/Method.gif) | [ICreateSpline2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~ICreateSpline2.html) | Creates a spline passing through the given points. |
| ![ Method](dotnetimages/Method.gif) | [ICreateSplineByEqnParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~ICreateSplineByEqnParams.html) | Creates a B-curve from B-spline data; that is, a set of B-spline vertices (control points) and a knot vector. |
| ![ Method](dotnetimages/Method.gif) | [ICreateSplinesByEqnParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~ICreateSplinesByEqnParams.html) | Creates one or more spline segments using the B-curve parameters provided. |
| ![ Method](dotnetimages/Method.gif) | [IGetSketchBlockDefinitions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~IGetSketchBlockDefinitions.html) | Gets all of the block definitions. |
| ![ Method](dotnetimages/Method.gif) | [Insert3DSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~Insert3DSketch.html) | Inserts a new 3D sketch in a model or closes the active sketch. |
| ![ Method](dotnetimages/Method.gif) | [InsertExplodeLineSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InsertExplodeLineSketch.html) | Inserts or closes an explode line sketch in an exploded view. |
| ![ Method](dotnetimages/Method.gif) | [InsertSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InsertSketch.html) | Inserts a new sketch in the current part or assembly document. |
| ![ Method](dotnetimages/Method.gif) | [InsertSketchBlockInstance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InsertSketchBlockInstance.html) | Inserts a block instance at the specified location using the block definition. |
| ![ Method](dotnetimages/Method.gif) | [InsertSketchPicture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InsertSketchPicture.html) | Obsolete. Superseded by [ISketchManager::InsertSketchPicture2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InsertSketchPicture2.html). |
| ![ Method](dotnetimages/Method.gif) | [InsertSketchPicture2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InsertSketchPicture2.html) | Inserts a picture on the current drawing sketch. |
| ![ Method](dotnetimages/Method.gif) | [IntersectCurves](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~IntersectCurves.html) | Creates a sketched intersection curve. |
| ![ Method](dotnetimages/Method.gif) | [MakeSketchBlockFromFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~MakeSketchBlockFromFile.html) | Creates a block definition using the specified file. |
| ![ Method](dotnetimages/Method.gif) | [MakeSketchBlockFromSelected](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~MakeSketchBlockFromSelected.html) | Creates a block definition at the specified location from the selected entities. |
| ![ Method](dotnetimages/Method.gif) | [MakeSketchBlockFromSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~MakeSketchBlockFromSketch.html) | Creates a block definition at the specified location using all of the sketch entities in the active sketch. |
| ![ Method](dotnetimages/Method.gif) | [MakeSketchChain](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~MakeSketchChain.html) | Creates a sketch path using the selected entities. |
| ![ Method](dotnetimages/Method.gif) | [PerimeterCircle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~PerimeterCircle.html) | Draws a 3-point perimeter arc. |
| ![ Method](dotnetimages/Method.gif) | [ReverseEndPointTangent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~ReverseEndPointTangent.html) | Reverses the end point tangent direction of splines and arcs. |
| ![ Method](dotnetimages/Method.gif) | [RotateOrCopy3DAboutVector](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~RotateOrCopy3DAboutVector.html) | Rotates, and optionally copies, the selected 3D sketch entities about the specified vector. |
| ![ Method](dotnetimages/Method.gif) | [RotateOrCopy3DAboutXYZ](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~RotateOrCopy3DAboutXYZ.html) | Rotates, and optionally copies, the selected 3D sketch entities about the specified x, y, and z coordinates. |
| ![ Method](dotnetimages/Method.gif) | [SetDynamicMirror](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SetDynamicMirror.html) | Enables or disables dynamic sketch mirroring, which is the automatic mirroring of newly created sketch entities about a selected centerline. |
| ![ Method](dotnetimages/Method.gif) | [SetGridOptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SetGridOptions.html) | Sets the options for the grid. |
| ![ Method](dotnetimages/Method.gif) | [SketchExtend](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchExtend.html) | Adds to the length of the selected sketch entity (i.e., line, centerline, or arc) to meet the nearest sketch entity. |
| ![ Method](dotnetimages/Method.gif) | [SketchOffset](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchOffset.html) | Obsolete. Superseded by [ISketchManager::SketchOffset2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchOffset2.html). |
| ![ Method](dotnetimages/Method.gif) | [SketchOffset2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchOffset2.html) | Offsets the selected sketch entities. |
| ![ Method](dotnetimages/Method.gif) | [SketchReplace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchReplace.html) | Obsolete. Superseded by [ISketchManager::SketchReplace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchReplace2.html). |
| ![ Method](dotnetimages/Method.gif) | [SketchReplace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchReplace2.html) | Replaces a sketch entity in a model with another sketch entity, preserving all references. |
| ![ Method](dotnetimages/Method.gif) | [SketchTrim](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchTrim.html) | Trims the selected sketch entities. |
| ![ Method](dotnetimages/Method.gif) | [SketchUseEdge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchUseEdge.html) | Obsolete. Superseded by [ISketchManager::SketchUseEdge2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchUseEdge2.html). |
| ![ Method](dotnetimages/Method.gif) | [SketchUseEdge2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchUseEdge2.html) | Obsolete. Superseded by [ISketchManager::SketchUseEdge3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchUseEdge3.html). |
| ![ Method](dotnetimages/Method.gif) | [SketchUseEdge3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchUseEdge3.html) | Creates sketch entities on a sketch plane by projecting selected edges, loops, faces, curves, and external sketch contours. |
| ![ Method](dotnetimages/Method.gif) | [SplitClosedSegment](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SplitClosedSegment.html) | Splits the selected closed sketch segment into two sketch segments. |
| ![ Method](dotnetimages/Method.gif) | [SplitOpenSegment](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SplitOpenSegment.html) | Splits the selected open sketch segment into two sketch segments. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)