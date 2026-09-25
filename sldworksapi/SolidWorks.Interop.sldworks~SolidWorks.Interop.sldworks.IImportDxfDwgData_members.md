<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IImportDxfDwgData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IImportDxfDwgData Interface |

The following tables list the members exposed by [IImportDxfDwgData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AddSketchConstraints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~AddSketchConstraints.html) | Gets or sets whether constraints are added to the geometry in the part sketch after importing the entities. |
| ![ Property](dotnetimages/Property.gif) | [DocumentTemplate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~DocumentTemplate.html) | Gets or sets the filename of the document template. |
| ![ Property](dotnetimages/Property.gif) | [IgnorePolylineWidth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~IgnorePolylineWidth.html) | Gets or sets whether to convert width polylines to solid fill hatches when importing to the part sketch. |
| ![ Property](dotnetimages/Property.gif) | [ImportDimensions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~ImportDimensions.html) | Gets or sets whether to import dimension into the part sketch. |
| ![ Property](dotnetimages/Property.gif) | [ImportHatch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~ImportHatch.html) | Gets or sets whether to import hatch into this part sketch. |
| ![ Property](dotnetimages/Property.gif) | [ImportMethod](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~ImportMethod.html) | Gets or sets whether to import this sheet (layout). |
| ![ Property](dotnetimages/Property.gif) | [LengthUnit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~LengthUnit.html) | Gets or sets the length units for the drawing. |
| ![ Property](dotnetimages/Property.gif) | [SheetName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SheetName.html) | Gets or sets the name of the sheet for the drawing. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetImportLayerToSheetFormat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetImportLayerToSheetFormat.html) | Gets whether the specified visible layer is imported to the drawing sheet or sheet format. |
| ![ Method](dotnetimages/Method.gif) | [GetImportLayerVisibility](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetImportLayerVisibility.html) | Gets whether the specified layer is imported hidden or visible. |
| ![ Method](dotnetimages/Method.gif) | [GetMergeDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetMergeDistance.html) | Gets whether points that are within the specified distance are merged in the part sketch after entities are imported. |
| ![ Method](dotnetimages/Method.gif) | [GetMergePoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetMergePoints.html) | Gets whether near-identical points are merged in the part sketch after entities are imported. |
| ![ Method](dotnetimages/Method.gif) | [GetPaperSize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetPaperSize.html) | Gets the size of the paper for the drawing. |
| ![ Method](dotnetimages/Method.gif) | [GetPosition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetPosition.html) | Gets the position of the entities created in the drawing. |
| ![ Method](dotnetimages/Method.gif) | [GetSheetScale](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetSheetScale.html) | Gets the sheet scale for the drawing. |
| ![ Method](dotnetimages/Method.gif) | [SetImportLayerToSheetFormat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetImportLayerToSheetFormat.html) | Sets whether the specified visible layers are imported to the sheet format or drawing sheet. |
| ![ Method](dotnetimages/Method.gif) | [SetImportLayerVisibility](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetImportLayerVisibility.html) | Sets whether the specified layers are imported hidden or visible. |
| ![ Method](dotnetimages/Method.gif) | [SetMergePoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetMergePoints.html) | Sets whether near-identical points within the specified distance are merged in the part sketch after entities are imported. |
| ![ Method](dotnetimages/Method.gif) | [SetPaperSize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetPaperSize.html) | Sets the size of the paper in the drawing. |
| ![ Method](dotnetimages/Method.gif) | [SetPosition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetPosition.html) | Sets the position of the entities created in the drawing. |
| ![ Method](dotnetimages/Method.gif) | [SetSheetScale](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetSheetScale.html) | Sets the sheet scale for the drawing. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IImportIgesData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportIgesData.html)