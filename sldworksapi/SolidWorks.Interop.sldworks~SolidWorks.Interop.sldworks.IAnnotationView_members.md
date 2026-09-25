<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAnnotationView Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IAnnotationView Interface |

The following tables list the members exposed by [IAnnotationView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Always2D](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~Always2D.html) | Gets whether to display annotations in 2D or 3D. |
| ![ Property](dotnetimages/Property.gif) | [AngleMadeWithViewHorizontal](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~AngleMadeWithViewHorizontal.html) | Gets the angle used to make the annotation view horizontal. |
| ![ Property](dotnetimages/Property.gif) | [AnnotationCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~AnnotationCount.html) | Gets the number of [annotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html) in this annotation view. |
| ![ Property](dotnetimages/Property.gif) | [Annotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~Annotations.html) | Obsolete. Superseded by [IAnnotationView::GetAnnotations2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~GetAnnotations2.html). |
| ![ Property](dotnetimages/Property.gif) | [FlatPatternView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~FlatPatternView.html) | Gets whether this annotation view is a flat-pattern view. |
| ![ Property](dotnetimages/Property.gif) | [UnassignedView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~UnassignedView.html) | Gets whether this annotation view is assigned to a 3D View. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [Activate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~Activate.html) | Activates this annotation view. |
| ![ Method](dotnetimages/Method.gif) | [ActivateAndReorient](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~ActivateAndReorient.html) | Activates and reorients this annotation view. |
| ![ Method](dotnetimages/Method.gif) | [GetAnnotations2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~GetAnnotations2.html) | Gets the annotations in this annotation view. |
| ![ Method](dotnetimages/Method.gif) | [GetViewRotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~GetViewRotation.html) | Gets the rotation matrix of the annotation view relative to the X-Y plane of the model. |
| ![ Method](dotnetimages/Method.gif) | [Hide](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~Hide.html) | Hides the annotations in an annotation view that is not activated. |
| ![ Method](dotnetimages/Method.gif) | [IGetAnnotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~IGetAnnotations.html) | Obsolete. Superseded by [IAnnotationView::GetAnnotations2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~GetAnnotations2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetViewRotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~IGetViewRotation.html) | Gets the rotation matrix of the annotation view relative to the X-Y plane of the model. |
| ![ Method](dotnetimages/Method.gif) | [IsShown](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~IsShown.html) | Gets whether the annotations in this annotation view are shown. |
| ![ Method](dotnetimages/Method.gif) | [MoveAnnotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~MoveAnnotations.html) | Moves the specified annotations to this annotation view. |
| ![ Method](dotnetimages/Method.gif) | [Orient](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~Orient.html) | Orients this annotation view. |
| ![ Method](dotnetimages/Method.gif) | [Show](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~Show.html) | Shows the annotations in an annotation view that is not activated. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotationView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)