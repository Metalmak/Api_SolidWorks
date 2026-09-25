<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ITablePatternFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ITablePatternFeatureData Interface |

The following tables list the members exposed by [ITablePatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CoordinateSystem](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~CoordinateSystem.html) | Gets or sets the coordinate system of the table-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [GeometryPattern](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~GeometryPattern.html) | Gets or sets whether to create the pattern using only the geometry (faces and edges) of the features for the table-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PatternBodyArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~PatternBodyArray.html) | Gets or sets the seed bodies to pattern for this table-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PatternFaceArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~PatternFaceArray.html) | Gets or sets the patterned faces for this table-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PatternFeatureArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~PatternFeatureArray.html) | Gets or sets the seed features used to create the table-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PointArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~PointArray.html) | Gets or sets the array of points that describe the x,y, and z locations of the repeating elements in the table-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PropagateVisualProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~PropagateVisualProperty.html) | Gets or sets whether to propagate visual properties (e.g., colors, textures, etc.) in the table-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [ReferencePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~ReferencePoint.html) | Gets or sets the reference point for pattern instances of this table-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [SkippedItemArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~SkippedItemArray.html) | Gets or sets the skipped items for this table-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [UseCentroid](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~UseCentroid.html) | Gets or sets whether to set the reference point to the centroid of the seed feature for this table-driven pattern feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~AccessSelections.html) | Gains access to selections used to define the table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetBasePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~GetBasePoint.html) | Gets the base point for this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPatternBodyCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~GetPatternBodyCount.html) | Gets the number of seed bodies for this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPatternFaceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~GetPatternFaceCount.html) | Gets the number of patterned faces in this table-driven feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPatternFeatureCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~GetPatternFeatureCount.html) | Gets the number of distinct seed features used to create this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPointCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~GetPointCount.html) | Gets the number of x, y, and z locations of the repeating elements in this table-driven pattern. |
| ![ Method](dotnetimages/Method.gif) | [GetReferencePointType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~GetReferencePointType.html) | Gets whether the table-driven pattern's reference point is a closed curve, a sketch point, or a vertex. |
| ![ Method](dotnetimages/Method.gif) | [GetSkippedItemCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~GetSkippedItemCount.html) | Gets the number of skipped items in this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~GetTransform.html) | Gets the transform for the specified repeating element in this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~IAccessSelections.html) | Obsolete. Superseded by [ITablePatternFeatureData::IAccessSelections2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITablePatternFeatureData~IAccessSelections2.html). |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~IAccessSelections2.html) | Gains access to selections used to define the table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetBasePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~IGetBasePoint.html) | Gets the base point for this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetPatternBodyArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~IGetPatternBodyArray.html) | Gets the seed bodies for this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetPatternFaceArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~IGetPatternFaceArray.html) | Gets the patterned faces in this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetPatternFeatureArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~IGetPatternFeatureArray.html) | Gets the seed features used to create the table-driven pattern. |
| ![ Method](dotnetimages/Method.gif) | [IGetPointArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~IGetPointArray.html) | Gets an array of doubles that describe the x, y, and z locations of the repeating elements in this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetSkippedItemArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~IGetSkippedItemArray.html) | Gets the skipped items in this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetPatternBodyArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~ISetPatternBodyArray.html) | Sets the seed bodies for this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetPatternFaceArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~ISetPatternFaceArray.html) | Sets the patterned faces for this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetPatternFeatureArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~ISetPatternFeatureArray.html) | Sets the seed features used to create the table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetPointArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~ISetPointArray.html) | Sets the points that describe the x, y, and z locations of the repeating elements in the table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetSkippedItemArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~ISetSkippedItemArray.html) | Sets the skipped items in this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [LoadPointsFromFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~LoadPointsFromFile.html) | Loads the location points of the table-driven pattern from a \*.sldptab file. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections that created this table-driven pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [SavePointsToFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData~SavePointsToFile.html) | Saves the location of the table-driven pattern feature's points to a \*.sldptab file. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ITablePatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)