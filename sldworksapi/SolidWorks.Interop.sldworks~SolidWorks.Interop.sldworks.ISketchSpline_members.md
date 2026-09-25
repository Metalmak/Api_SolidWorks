<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISketchSpline Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISketchSpline Interface |

The following tables list the members exposed by [ISketchSpline](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CurveDegree](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~CurveDegree.html) | Gets or sets the degree of curve for this Bezier curve style spline. |
| ![ Property](dotnetimages/Property.gif) | [CurveType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~CurveType.html) | Gets or sets the type of curve for this style spline. |
| ![ Property](dotnetimages/Property.gif) | [DisplayControlPolygon](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~DisplayControlPolygon.html) | Gets or sets whether to add a control polygon to this spline. |
| ![ Property](dotnetimages/Property.gif) | [IsRationalCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~IsRationalCurve.html) | Gets whether this spline is rational or non-rational. |
| ![ Property](dotnetimages/Property.gif) | [IsStyleSpline](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~IsStyleSpline.html) | Gets whether this spline is a style spline. |
| ![ Property](dotnetimages/Property.gif) | [Proportional](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~Proportional.html) | Gets or sets whether the spline resizes proportionally when you drag an endpoint the spline. |
| ![ Property](dotnetimages/Property.gif) | [ShowCurvatureCombs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~ShowCurvatureCombs.html) | Gets or sets whether to show curvature combs. |
| ![ Property](dotnetimages/Property.gif) | [ShowInflectionPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~ShowInflectionPoints.html) | Gets or sets whether show the inflection points of this spline. |
| ![ Property](dotnetimages/Property.gif) | [ShowMinimumRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~ShowMinimumRadius.html) | Gets or sets the minimum radius of a curve for this spline. |
| ![ Property](dotnetimages/Property.gif) | [ShowSplineHandles](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~ShowSplineHandles.html) | Gets or sets whether to show the [handles](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISplineHandle.html) for this spline. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddCurvatureControl](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~AddCurvatureControl.html) | Adds a curvature control pointer to this spline. |
| ![ Method](dotnetimages/Method.gif) | [AddTangencyControl](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~AddTangencyControl.html) | Adds a new handle to help control the tangency of this spline. |
| ![ Method](dotnetimages/Method.gif) | [DeletePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~DeletePoint.html) | Deletes a point on this spline. |
| ![ Method](dotnetimages/Method.gif) | [GetControlVertexWeights](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~GetControlVertexWeights.html) | Gets the weights of the control vetexes of this rational spline. |
| ![ Method](dotnetimages/Method.gif) | [GetEquationParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~GetEquationParameters.html) | Obsolete. Superseded by [ISketchSpline::GetEquationParameters2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSpline~GetEquationParameters2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetEquationParameters2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~GetEquationParameters2.html) | Gets an equation-driven curve's parameters. |
| ![ Method](dotnetimages/Method.gif) | [GetPointCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~GetPointCount.html) | Gets the number of points in this sketch spline segment. |
| ![ Method](dotnetimages/Method.gif) | [GetPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~GetPoints.html) | Obsolete. Superseded by [ISketchSpline::GetPoints2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSpline~GetPoints2.html) and [ISketchSpline::IEnumPoints](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSpline~IEnumPoints.html). |
| ![ Method](dotnetimages/Method.gif) | [GetPoints2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~GetPoints2.html) | Gets an array of sketch points for the spline. |
| ![ Method](dotnetimages/Method.gif) | [GetSplineHandleCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~GetSplineHandleCount.html) | Gets the number of [handles](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISplineHandle.html) in this spline. |
| ![ Method](dotnetimages/Method.gif) | [GetSplineHandles](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~GetSplineHandles.html) | Gets the handles of this spline. |
| ![ Method](dotnetimages/Method.gif) | [IEnumPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~IEnumPoints.html) | Gets an enumeration of sketch points for the spline. |
| ![ Method](dotnetimages/Method.gif) | [IGetPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~IGetPoints.html) | Obsolete. Superseded by [ISketchSpline::GetPoints2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSpline~GetPoints2.html) and [ISketchSpline::IEnumPoints](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSpline~IEnumPoints.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetSplineHandles](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~IGetSplineHandles.html) | Gets the handles of this spline. |
| ![ Method](dotnetimages/Method.gif) | [InsertPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~InsertPoint.html) | Inserts a point at the specified coordinates of this spline. |
| ![ Method](dotnetimages/Method.gif) | [MakeRational](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~MakeRational.html) | Sets whether this spline is rational or non-rational. |
| ![ Method](dotnetimages/Method.gif) | [ModifyControlPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~ModifyControlPoint.html) | Specifies new coordinates for the specified control point of this sketch spline. |
| ![ Method](dotnetimages/Method.gif) | [ModifyKnot](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~ModifyKnot.html) | Modifies the specified interior knot of this sketch spline. |
| ![ Method](dotnetimages/Method.gif) | [RelaxSpline](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~RelaxSpline.html) | Smoothens the shape of a spline that was changed by dragging a node on a [control polygon](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSpline~DisplayControlPolygon.html). |
| ![ Method](dotnetimages/Method.gif) | [ResetAllHandles](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~ResetAllHandles.html) | Resets all [handles](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISplineHandle.html) to their initial state. |
| ![ Method](dotnetimages/Method.gif) | [SetControlVertexWeights](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~SetControlVertexWeights.html) | Sets the weights of the control vetexes of this rational spline. |
| ![ Method](dotnetimages/Method.gif) | [SetEquationParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~SetEquationParameters.html) | Obsolete. Superseded by [ISketchSpline::SetEquationParameters2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSpline~SetEquationParameters2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetEquationParameters2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~SetEquationParameters2.html) | Sets an equation-driven curve's parameters. |
| ![ Method](dotnetimages/Method.gif) | [Simplify](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~Simplify.html) | Reduces the number of points in a spline to increase system performance in models with complex spline curves. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSpline Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ISplineHandle Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplineHandle.html)

[ISplineParamData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplineParamData.html)