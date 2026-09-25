<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IRefPlaneFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IRefPlaneFeatureData Interface |

The following tables list the members exposed by [IRefPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Angle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~Angle.html) | Gets or sets the angle of the reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [AngleOrDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~AngleOrDistance.html) | Gets or sets the angle or distance of the specified [reference](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPlaneFeatureData~Reference.html) for this reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [AutoSize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~AutoSize.html) | Gets or sets whether to automatically size the reference plane feature to either the geometry on which it is created or to the bounding box of the model geometry. |
| ![ Property](dotnetimages/Property.gif) | [Constraint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~Constraint.html) | Gets or sets the constraint for the specified [reference](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPlaneFeatureData~Reference.html) for this reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [Distance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~Distance.html) | Gets or sets the distance, in meters, to offset the reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [OriginOnCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~OriginOnCurve.html) | Gets or sets whether to place the origin on the curve for this reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [ProjectionType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~ProjectionType.html) | Gets or sets the projection type for this on-surface reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [Reference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~Reference.html) | Gets or sets the reference entity for the specified reference for this reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [ReverseDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~ReverseDirection.html) | Obsolete. Superseded by [IRefPlaneFeatureData::ReversedReferenceDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~ReversedReferenceDirection.html). |
| ![ Property](dotnetimages/Property.gif) | [ReversedReferenceDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~ReversedReferenceDirection.html) | Gets or sets whether to reverse the direction of the specified reference for this reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [Selections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~Selections.html) | Gets or sets the selected entities used to create the reference plane feature or sets the entities to use to create the reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [SolutionIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~SolutionIndex.html) | Gets or sets the intended plane when there are multiple planes from which to select for an on-surface reference plane feature. |
| ![ Property](dotnetimages/Property.gif) | [Type](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~Type.html) | Gets the type of reference plane created in SOLIDWORKS 2009 or earlier. Can also get whether a constraint-based reference plane created in SOLIDWORKS 2010 or has angle or offset distance references.   **NOTE:** **This property is a get-only property.** **Set is not implemented**. |
| ![ Property](dotnetimages/Property.gif) | [Type2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~Type2.html) | Gets whether the reference plane is constraint based; thus, created in SOLIDWORKS 2010 and later.  **NOTE:** **This property is a get-only property.** **Set is not implemented**. |
| ![ Property](dotnetimages/Property.gif) | [UpdatePlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~UpdatePlane.html) | Gets or sets whether to update this reference plane so that it is parallel to the screen. |
| ![ Property](dotnetimages/Property.gif) | [UseNormalPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~UseNormalPlane.html) | Gets or sets whether to:   * Use the plane normal to the selected plane * Automatically size the plane to either the geometry on which it is created or to the bounding box of the model geometry |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~AccessSelections.html) | Gains access to the selections that define a reference plane feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSelectionsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~GetSelectionsCount.html) | Gets the number of entities selected to create this reference plane feature. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~IAccessSelections.html) | Gains access to the selections that define a reference plane feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~IGetSelections.html) | Gets the selected entities used to create this reference plane feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~ISetSelections.html) | Sets the entities to use to create the reference plane feature. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections that created the reference plane feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IRefPlaneFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IRefPlane Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html)