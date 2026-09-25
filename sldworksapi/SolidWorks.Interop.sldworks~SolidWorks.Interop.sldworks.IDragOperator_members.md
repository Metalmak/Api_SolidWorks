<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDragOperator Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IDragOperator Interface |

The following tables list the members exposed by [IDragOperator](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [ApplyToThisConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~ApplyToThisConfiguration.html) | Gets or sets the configurations to which to apply the movement of the components. |
| ![ Property](dotnetimages/Property.gif) | [Clearance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~Clearance.html) | Gets the clearance distance between the components. |
| ![ Property](dotnetimages/Property.gif) | [CollisionDetectionEnabled](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~CollisionDetectionEnabled.html) | Gets or sets the collision detection setting. |
| ![ Property](dotnetimages/Property.gif) | [DragCorrected](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~DragCorrected.html) | Gets whether or not the drag operation was corrected. |
| ![ Property](dotnetimages/Property.gif) | [DragMode](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~DragMode.html) | Gets or sets the drag mode for this drag operation. |
| ![ Property](dotnetimages/Property.gif) | [DynamicClearanceEnabled](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~DynamicClearanceEnabled.html) | Gets or sets the dynamic clearance setting. |
| ![ Property](dotnetimages/Property.gif) | [GraphicsRedrawEnabled](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~GraphicsRedrawEnabled.html) | Gets or sets whether or not to update the graphics display after moving components. |
| ![ Property](dotnetimages/Property.gif) | [HearClashes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~HearClashes.html) | Gets or sets whether sound is associated with entity clashes. |
| ![ Property](dotnetimages/Property.gif) | [HighlightClashes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~HighlightClashes.html) | Gets or sets whether to highlight clashes. |
| ![ Property](dotnetimages/Property.gif) | [IgnoreComplexSurfaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~IgnoreComplexSurfaces.html) | Gets or sets whether complex surfaces are ignored. |
| ![ Property](dotnetimages/Property.gif) | [IsDragByRay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~IsDragByRay.html) | Gets or sets the drag-by-ray setting. |
| ![ Property](dotnetimages/Property.gif) | [IsDragSpecific](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~IsDragSpecific.html) | Gets or sets the drag-specific setting. |
| ![ Property](dotnetimages/Property.gif) | [IsRelaxationEval](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~IsRelaxationEval.html) | Gets or sets the relaxation evaluation. |
| ![ Property](dotnetimages/Property.gif) | [SmartMating](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~SmartMating.html) | Gets or sets SmartMates. |
| ![ Property](dotnetimages/Property.gif) | [TransformType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~TransformType.html) | Gets or sets the type of transformation. |
| ![ Property](dotnetimages/Property.gif) | [UseAbsoluteTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~UseAbsoluteTransform.html) | Gets or sets whether the transforms to use with [IDragOperator::Drag](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDragOperator~Drag.html) or [IDragOperator::IDrag](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDragOperator~IDrag.html) are absolute or relative. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~AddComponent.html) | Adds a component to the list of components to drag. |
| ![ Method](dotnetimages/Method.gif) | [AddDynamicClearance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~AddDynamicClearance.html) | Adds a dynamic clearance detector. |
| ![ Method](dotnetimages/Method.gif) | [BeginDrag](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~BeginDrag.html) | Initiates the drag operation. |
| ![ Method](dotnetimages/Method.gif) | [CollisionDetection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~CollisionDetection.html) | Sets the collision detection parameters. |
| ![ Method](dotnetimages/Method.gif) | [Drag](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~Drag.html) | Sets the transform matrix for this drag operation. |
| ![ Method](dotnetimages/Method.gif) | [DragAsUI](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~DragAsUI.html) | Sets the transform matrix for this drag operation. |
| ![ Method](dotnetimages/Method.gif) | [EndDrag](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~EndDrag.html) | Terminates the drag operation. |
| ![ Method](dotnetimages/Method.gif) | [GetDragPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~GetDragPoint.html) | Gets the drag point. |
| ![ Method](dotnetimages/Method.gif) | [IAddComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~IAddComponent.html) | Adds a component to the list of components to drag. |
| ![ Method](dotnetimages/Method.gif) | [IAddDynamicClearance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~IAddDynamicClearance.html) | Adds a dynamic clearance detector. |
| ![ Method](dotnetimages/Method.gif) | [ICollisionDetection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~ICollisionDetection.html) | Sets the collision detection parameters. |
| ![ Method](dotnetimages/Method.gif) | [IDrag](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~IDrag.html) | Sets the transform matrix for this drag operation. |
| ![ Method](dotnetimages/Method.gif) | [IGetDragPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~IGetDragPoint.html) | Gets the drag point. |
| ![ Method](dotnetimages/Method.gif) | [ISetDragPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~ISetDragPoint.html) | Sets the drag point. |
| ![ Method](dotnetimages/Method.gif) | [SetDragPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~SetDragPoint.html) | Sets the drag point. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IDragOperator Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)