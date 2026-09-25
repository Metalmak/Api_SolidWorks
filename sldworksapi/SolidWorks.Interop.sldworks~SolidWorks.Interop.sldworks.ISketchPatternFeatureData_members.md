<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISketchPatternFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISketchPatternFeatureData Interface |

The following tables list the members exposed by [ISketchPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AutoSelect](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~AutoSelect.html) | Gets whether to automatically select all bodies in a multibody part intersected by this sketch-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [BodyPattern](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~BodyPattern.html) | Gets or sets whether to base this sketch pattern feature on bodies or features and faces. |
| ![ Property](dotnetimages/Property.gif) | [FeatureScope](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~FeatureScope.html) | Gets which bodies in this multibody part are affected by this sketch-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [FeatureScopeBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~FeatureScopeBodies.html) | Gets the bodies in this multibody part to be affected by this sketch-driven pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [GeometryPattern](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~GeometryPattern.html) | Gets or sets whether to create the pattern using only the geometry (faces and edges) of the feature. |
| ![ Property](dotnetimages/Property.gif) | [PatternBodyArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~PatternBodyArray.html) | Gets and sets the bodies to pattern for this sketch pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PatternElement](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~PatternElement.html) | Gets or sets the type of entities to base this sketch pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PatternFaceArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~PatternFaceArray.html) | Gets or sets the patterned faces for the sketch pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PatternFeatureArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~PatternFeatureArray.html) | Gets or sets the seed features for the sketch pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [PropagateVisualProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~PropagateVisualProperty.html) | Gets or sets whether to propagate visual properties (i.e., colors to all pattern instances). |
| ![ Property](dotnetimages/Property.gif) | [ReferencePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~ReferencePoint.html) | Gets or sets the reference point for this sketch pattern feature. |
| ![ Property](dotnetimages/Property.gif) | [Sketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~Sketch.html) | Gets or sets the sketch from which that this sketch pattern feature is created. |
| ![ Property](dotnetimages/Property.gif) | [UseCentroid](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~UseCentroid.html) | Gets or sets whether to use a centroid for this sketch pattern feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~AccessSelections.html) | Gains access to selections used to define the sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetBasePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~GetBasePoint.html) | Gets the base point data from which this sketch pattern is created. |
| ![ Method](dotnetimages/Method.gif) | [GetPatternBodyCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~GetPatternBodyCount.html) | Gets the number of seed bodies in the sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPatternFaceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~GetPatternFaceCount.html) | Gets the number of patterned faces. |
| ![ Method](dotnetimages/Method.gif) | [GetPatternFeatureCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~GetPatternFeatureCount.html) | Gets the number of seed features for this sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetReferencePointType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~GetReferencePointType.html) | Gets the type of reference point for this sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~GetTransform.html) | Gets the transform for the specified instance of this sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~IAccessSelections.html) | Obsolete. Superseded by [ISketchPatternFeatureData::IAccessSelections2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchPatternFeatureData~IAccessSelections2.html). |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~IAccessSelections2.html) | Gains access to selections used to define the sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetBasePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~IGetBasePoint.html) | Gets the base point data from which this sketch pattern is created. |
| ![ Method](dotnetimages/Method.gif) | [IGetPatternBodyArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~IGetPatternBodyArray.html) | Gets the seed bodies for the sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetPatternFaceArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~IGetPatternFaceArray.html) | Gets the patterned faces for the sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetPatternFeatureArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~IGetPatternFeatureArray.html) | Gets the seed features for the sketch pattern. |
| ![ Method](dotnetimages/Method.gif) | [ISetPatternBodyArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~ISetPatternBodyArray.html) | Sets the seed bodies for the sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetPatternFaceArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~ISetPatternFaceArray.html) | Sets the patterned faces for the sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetPatternFeatureArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~ISetPatternFeatureArray.html) | Sets the seed features for the sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections that created this sketch pattern feature. |
| ![ Method](dotnetimages/Method.gif) | [SetFeatureScope](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~SetFeatureScope.html) | Sets the feature scope, whether to autoselect the affected bodies, and the affected bodies in this sketch pattern feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)