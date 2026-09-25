<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IClosedCornerFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IClosedCornerFeatureData Interface |

The following tables list the members exposed by [IClosedCornerFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CornerType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~CornerType.html) | Gets or sets the closed corner type. |
| ![ Property](dotnetimages/Property.gif) | [Faces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~Faces.html) | Gets or sets the faces for this closed corner feature. |
| ![ Property](dotnetimages/Property.gif) | [GapDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~GapDistance.html) | Gets or sets the distance for the gap in a closed corner in a sheet metal part. |
| ![ Property](dotnetimages/Property.gif) | [OpenBendRegion](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~OpenBendRegion.html) | Gets or sets whether this closed corner has an open bend region. |
| ![ Property](dotnetimages/Property.gif) | [OverlapUnderlapRatio](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~OverlapUnderlapRatio.html) | Gets or sets the overlap/underlap ratio for this closed corner. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~AccessSelections.html) | Gains access to the selections that define this closed corner feature. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~IAccessSelections.html) | Obsolete. Superseded by [IClosedCornerFeatureData::IAccessSelections2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IClosedCornerFeatureData~IAccessSelections2.html). |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~IAccessSelections2.html) | Gains access to the selections that describe this closed corner feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~IGetFaces.html) | Gets the faces for this closed corner feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetFacesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~IGetFacesCount.html) | Gets the number of faces in this closed corner feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~ISetFaces.html) | Sets the faces for this closed corner feature. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData~ReleaseSelectionAccess.html) | Releases access to selections that describe this closed corner feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IClosedCornerFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IClosedCornerFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IModelDoc2::InsertSheetMetalClosedCorner Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSheetMetalClosedCorner.html)