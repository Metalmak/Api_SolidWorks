<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IVariableFilletFeatureData2 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IVariableFilletFeatureData2 Interface |

The following tables list the members exposed by [IVariableFilletFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AsymmetricFillet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~AsymmetricFillet.html) | Gets or sets whether this variable radius fillet is asymmetric. |
| ![ Property](dotnetimages/Property.gif) | [ConicTypeForCrossSectionProfile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~ConicTypeForCrossSectionProfile.html) | Gets or sets the type of profile for this fillet. |
| ![ Property](dotnetimages/Property.gif) | [CurvatureContinuous](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~CurvatureContinuous.html) | Gets or sets whether to create a smoother curvature between adjacent surfaces for this variable radius fillet feature. |
| ![ Property](dotnetimages/Property.gif) | [DefaultConicRhoOrRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~DefaultConicRhoOrRadius.html) | Gets or sets the default conic rho or conic radius of this fillet. |
| ![ Property](dotnetimages/Property.gif) | [DefaultDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~DefaultDistance.html) | Gets or sets the default Distance 2 radius of this asymmetric fillet. |
| ![ Property](dotnetimages/Property.gif) | [DefaultRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~DefaultRadius.html) | Gets or sets the default radius for this symmetric fillet or the default Distance 1 radius for this asymmetric fillet. |
| ![ Property](dotnetimages/Property.gif) | [FilletEdgeCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~FilletEdgeCount.html) | Gets the number of edges to fillet. |
| ![ Property](dotnetimages/Property.gif) | [OverflowType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~OverflowType.html) | Gets or sets the overflow type for this variable fillet feature. |
| ![ Property](dotnetimages/Property.gif) | [PropagateFeatureToParts](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~PropagateFeatureToParts.html) | Gets or sets whether to extend the fillet feature to all affected parts in the assembly. |
| ![ Property](dotnetimages/Property.gif) | [PropagateToTangentFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~PropagateToTangentFaces.html) | Gets or sets whether to extend the fillet to all faces tangent to the selected face or edge. |
| ![ Property](dotnetimages/Property.gif) | [TransitionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~TransitionType.html) | Gets or sets the type of transition between this variable fillet and an adjacent fillet. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~AccessSelections.html) | Gains access to the selections used to define the variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [GetConicRhoOrRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetConicRhoOrRadius.html) | Gets the conic rho, conic radius, or circular radius of this fillet. |
| ![ Method](dotnetimages/Method.gif) | [GetConicRhoOrRadius2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetConicRhoOrRadius2.html) | Gets the conic rho or radius at the specified vertex. |
| ![ Method](dotnetimages/Method.gif) | [GetControlPointConicRhoOrRadiusAtIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetControlPointConicRhoOrRadiusAtIndex.html) | Gets the conic rho or radius at the specified control point. |
| ![ Method](dotnetimages/Method.gif) | [GetControlPointDistanceAtIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetControlPointDistanceAtIndex.html) | Gets the Distance 2 radius at the specified control point for the asymmetric fillet. |
| ![ Method](dotnetimages/Method.gif) | [GetControlPointRadiusAtIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetControlPointRadiusAtIndex.html) | Gets the radius at the specified control point. |
| ![ Method](dotnetimages/Method.gif) | [GetControlPointsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetControlPointsCount.html) | Gets the number of intermediate control points on this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [GetDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetDistance.html) | Gets the Distance 2 radius for this asymmetric fillet. |
| ![ Method](dotnetimages/Method.gif) | [GetFilletEdgeAtIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetFilletEdgeAtIndex.html) | Gets the fillet edge at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [GetRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetRadius.html) | Obsolete. Superseded by [IVariableFilletFeatureData2::GetRadius2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVariableFilletFeatureData2~GetRadius2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetRadius2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetRadius2.html) | Gets the value of the Distance 1 radius at the specified vertex. |
| ![ Method](dotnetimages/Method.gif) | [GetSetbackDistanceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetSetbackDistanceCount.html) | Gets the number of setback distances for the specified vertex on this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSetbackVertexDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetSetbackVertexDistance.html) | Gets the setback distance for the specified vertex on this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSetbackVertices](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetSetbackVertices.html) | Gets the setback vertices for this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSetbackVerticesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetSetbackVerticesCount.html) | Gets the number of setback vertices for this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~IAccessSelections.html) | Gains access to the selections used to define the variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetConicRhoOrRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~IGetConicRhoOrRadius.html) | Gets the conic rho, conic radius, or circular radius of this fillet. |
| ![ Method](dotnetimages/Method.gif) | [IGetFilletEdgeAtIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~IGetFilletEdgeAtIndex.html) | Gets the fillet edge at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [IGetRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~IGetRadius.html) | Obsolete. Superseded by [IVariableFilletFeatureData2::Radius2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVariableFilletFeatureData2~GetRadius2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetSetbackVertexDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~IGetSetbackVertexDistance.html) | Gets the setback distance for the specified vertex on this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetSetbackVertices](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~IGetSetbackVertices.html) | Gets the setback vertices for this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetConicRhoOrRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~ISetConicRhoOrRadius.html) | Sets the conic rho, conic radius, or circular radius of this fillet. |
| ![ Method](dotnetimages/Method.gif) | [ISetRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~ISetRadius.html) | Sets the radius value for specified fillet item. |
| ![ Method](dotnetimages/Method.gif) | [ISetSetbackVertexDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~ISetSetbackVertexDistance.html) | Sets the setback distance for the specified vertex and its edges on this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetSetbackVertices](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~ISetSetbackVertices.html) | Sets the setback vertices for this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~ReleaseSelectionAccess.html) | Releases access to the selections used to define the variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [SetConicRhoOrRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~SetConicRhoOrRadius.html) | Sets the conic rho or radius for the specified fillet item. |
| ![ Method](dotnetimages/Method.gif) | [SetControlPointConicRhoOrRadiusAtIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~SetControlPointConicRhoOrRadiusAtIndex.html) | Sets the conic rho or radius at the specified control point. |
| ![ Method](dotnetimages/Method.gif) | [SetControlPointDistanceAtIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~SetControlPointDistanceAtIndex.html) | Sets the Distance 2 radius at the specified control point for the asymmetric fillet. |
| ![ Method](dotnetimages/Method.gif) | [SetControlPointRadiusAtIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~SetControlPointRadiusAtIndex.html) | Sets the radius at the specified control point. |
| ![ Method](dotnetimages/Method.gif) | [SetDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~SetDistance.html) | Sets the Distance 2 radius for this asymmetric fillet. |
| ![ Method](dotnetimages/Method.gif) | [SetRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~SetRadius.html) | Sets the value of the Distance 1 radius at the specified vertex. |
| ![ Method](dotnetimages/Method.gif) | [SetSetbackVertexDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~SetSetbackVertexDistance.html) | Sets the setback distances on fillet edges from the specified fillet corner vertex on this variable fillet feature. |
| ![ Method](dotnetimages/Method.gif) | [SetSetbackVertices](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~SetSetbackVertices.html) | Sets the setback vertices for this variable fillet feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IVariableFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ISimpleFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html)

[IChamferFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChamferFeatureData2.html)