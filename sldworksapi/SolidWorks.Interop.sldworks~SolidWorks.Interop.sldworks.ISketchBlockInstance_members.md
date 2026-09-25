<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISketchBlockInstance Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISketchBlockInstance Interface |

The following tables list the members exposed by [ISketchBlockInstance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Angle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~Angle.html) | Gets or sets the angle around the insertion point which to rotate this block instance. |
| ![ Property](dotnetimages/Property.gif) | [BlockToSketchTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~BlockToSketchTransform.html) | Gets all of the sketch entities from a block definition and transforms them to coordinates in sketch space. |
| ![ Property](dotnetimages/Property.gif) | [Definition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~Definition.html) | Gets or sets the block definition for this block instance. |
| ![ Property](dotnetimages/Property.gif) | [DimensionDisplay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~DimensionDisplay.html) | Gets whether dimensions are displayed. |
| ![ Property](dotnetimages/Property.gif) | [InstancePosition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~InstancePosition.html) | Gets or sets the position for this block instance. |
| ![ Property](dotnetimages/Property.gif) | [Layer](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~Layer.html) | Gets or sets the name of the layer where this block is located. |
| ![ Property](dotnetimages/Property.gif) | [LockAngle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~LockAngle.html) | Gets or sets whether the angle around the insertion point which to rotate this block instance is locked. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~Name.html) | Gets or sets the name of this block instance. |
| ![ Property](dotnetimages/Property.gif) | [Scale](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~Scale.html) | Obsolete. Superseded by [ISketchBlockInstance::Scale2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchBlockInstance~Scale2.html). |
| ![ Property](dotnetimages/Property.gif) | [Scale2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~Scale2.html) | Gets or sets the scale for this block instance. |
| ![ Property](dotnetimages/Property.gif) | [TextDisplay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~TextDisplay.html) | Gets or sets whether to display text for this block instance. |
| ![ Property](dotnetimages/Property.gif) | [Visible](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~Visible.html) | Gets or sets the visibility of this block instance. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetArrowHeadStyle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~GetArrowHeadStyle.html) | Gets the arrowhead style of the leader on this block instance. |
| ![ Method](dotnetimages/Method.gif) | [GetAttachedEntities](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~GetAttachedEntities.html) | Gets the entities to which this block instance is attached. |
| ![ Method](dotnetimages/Method.gif) | [GetAttributeCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~GetAttributeCount.html) | Gets the number of attributes for this block instance. |
| ![ Method](dotnetimages/Method.gif) | [GetAttributes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~GetAttributes.html) | Gets the attributes for this block instance. |
| ![ Method](dotnetimages/Method.gif) | [GetAttributeValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~GetAttributeValue.html) | Gets the value of the specified attribute for this block instance. |
| ![ Method](dotnetimages/Method.gif) | [GetLeaderPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~GetLeaderPoints.html) | Gets the coordinate information for the leader on this block instance. |
| ![ Method](dotnetimages/Method.gif) | [GetLeaderStyle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~GetLeaderStyle.html) | Gets the leader style of this block instance. |
| ![ Method](dotnetimages/Method.gif) | [GetSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~GetSketch.html) | Gets the sketch in which this block instance is present. |
| ![ Method](dotnetimages/Method.gif) | [IGetAttributes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~IGetAttributes.html) | Gets the attributes for this block instance. |
| ![ Method](dotnetimages/Method.gif) | [IGetLeaderPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~IGetLeaderPoints.html) | Gets the coordinate information for the leader on this block instance. |
| ![ Method](dotnetimages/Method.gif) | [Select](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~Select.html) | Selects and marks the block instance. |
| ![ Method](dotnetimages/Method.gif) | [SetAttributeValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~SetAttributeValue.html) | Sets the value of the specified attribute for this block instance. |
| ![ Method](dotnetimages/Method.gif) | [SetLeader](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~SetLeader.html) | Sets the leader style for this block instance. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchBlockInstance Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ISketchBlockDefinition Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockDefinition.html)

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)