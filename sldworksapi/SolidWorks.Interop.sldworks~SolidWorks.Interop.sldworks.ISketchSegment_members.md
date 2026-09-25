<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISketchSegment Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISketchSegment Interface |

The following tables list the members exposed by [ISketchSegment](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Color](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~Color.html) | Gets or sets the color of this sketch segment. Sketch segment color is only supported in drawing documents. |
| ![ Property](dotnetimages/Property.gif) | [ConstructionGeometry](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~ConstructionGeometry.html) | Gets or sets whether this sketch segment is construction geometry, for example, a centerline for a feature revolve operation. |
| ![ Property](dotnetimages/Property.gif) | [Layer](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~Layer.html) | gets or sets the layer used by this sketch segment. |
| ![ Property](dotnetimages/Property.gif) | [LayerOverride](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~LayerOverride.html) | Gets or sets whether the sketch segment has properties that override the default properties of the layer. |
| ![ Property](dotnetimages/Property.gif) | [Status](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~Status.html) | Gets the type of sketch constraint for this sketch segment.  **NOTE: This property is a get-only property. Set is not implemented.** |
| ![ Property](dotnetimages/Property.gif) | [Style](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~Style.html) | Gets or sets the line style for this sketch segment. |
| ![ Property](dotnetimages/Property.gif) | [Width](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~Width.html) | Gets or sets the line width for this sketch segment. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [CreateWireBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~CreateWireBody.html) | Creates a wire body using the selected sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [DeSelect](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~DeSelect.html) | Deselects the sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [EqualSegment](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~EqualSegment.html) | Divides this sketch segment into equally spaced sketch segments or points. |
| ![ Method](dotnetimages/Method.gif) | [GetConstraints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetConstraints.html) | Gets the constraints for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [GetCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetCurve.html) | Gets the underlying curve for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [GetID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetID.html) | Gets the for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [GetLength](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetLength.html) | Gets the length of this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [GetName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetName.html) | Gets the name of this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [GetRelations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetRelations.html) | Gets the sketch relations for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [GetRelationsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetRelationsCount.html) | Gets the number of sketch relations for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [GetSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetSketch.html) | Gets the sketch for the current sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPathCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetSketchPathCount.html) | Gets the number of sketch paths for this sketch segment |
| ![ Method](dotnetimages/Method.gif) | [GetSketchPaths](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetSketchPaths.html) | Gets the sketch paths for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [GetSketchSlot](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetSketchSlot.html) | Gets sketch slot with which this sketch segment is associated. |
| ![ Method](dotnetimages/Method.gif) | [GetType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetType.html) | Gets the type of sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [IGetConstraints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~IGetConstraints.html) | Gets the constraints for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [IGetConstraintsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~IGetConstraintsCount.html) | Gets the number of constraints on the sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [IGetCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~IGetCurve.html) | Gets the underlying curve for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [IGetID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~IGetID.html) | Gets the ID for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [IGetRelations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~IGetRelations.html) | Gets the sketch relations for this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [IGetSketchPaths](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~IGetSketchPaths.html) | Gets the sketch paths in this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [IsBendLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~IsBendLine.html) | Gets whether the sketch segment is a bendline. |
| ![ Method](dotnetimages/Method.gif) | [JogLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~JogLine.html) | Creates rectangular jog on the specified line. |
| ![ Method](dotnetimages/Method.gif) | [Select](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~Select.html) | Obsolete. Superseded by [ISketchSegment::Select4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment~Select4.html). |
| ![ Method](dotnetimages/Method.gif) | [Select2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~Select2.html) | Obsolete. Superseded by [ISketchSegment::Select4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment~Select4.html). |
| ![ Method](dotnetimages/Method.gif) | [Select3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~Select3.html) | Obsolete. Superseded by [ISketchSegment::Select4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment~Select4.html). |
| ![ Method](dotnetimages/Method.gif) | [Select4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~Select4.html) | Selects this sketch segment and marks it. |
| ![ Method](dotnetimages/Method.gif) | [SelectByMark](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~SelectByMark.html) | Obsolete. Superseded by [ISketchSegment::Select4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment~Select4.html). |
| ![ Method](dotnetimages/Method.gif) | [SelectChain](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~SelectChain.html) | Selects chains of entities attached to this sketch segment. |
| ![ Method](dotnetimages/Method.gif) | [SplitEntity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~SplitEntity.html) | Splits the selected sketch entity at the specified point. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)