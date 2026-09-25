<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IExplodeStep Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IExplodeStep Interface |

The following tables list the members exposed by [IExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AutoSpaceComponentsOnDrag](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~AutoSpaceComponentsOnDrag.html) | Gets or sets whether to automatically space a group of components equally along an axis as you drag them. |
| ![ Property](dotnetimages/Property.gif) | [DivergeDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~DivergeDirection.html) | Gets or sets the diverge direction entity for this radial explode step. |
| ![ Property](dotnetimages/Property.gif) | [DivergeFromAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~DivergeFromAxis.html) | Gets or sets whether to move components at an angle from the explode direction of this radial explode step. |
| ![ Property](dotnetimages/Property.gif) | [ExplodeDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~ExplodeDistance.html) | Gets or sets the distance to move components in this regular or radial explode step. |
| ![ Property](dotnetimages/Property.gif) | [ExplodeStepType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~ExplodeStepType.html) | Gets the type of this explode step. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~Name.html) | Gets or sets the name of this explode step. |
| ![ Property](dotnetimages/Property.gif) | [ReverseRotationDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~ReverseRotationDirection.html) | Gets or sets whether to reverse the direction of rotation of components in this regular explode step. |
| ![ Property](dotnetimages/Property.gif) | [ReverseTranslationDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~ReverseTranslationDirection.html) | Gets or sets whether to reverse the explode direction in this regular explode step. |
| ![ Property](dotnetimages/Property.gif) | [RotateAboutEachComponentOrigin](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~RotateAboutEachComponentOrigin.html) | Gets or sets whether components rotate about their origins in this regular explode step. |
| ![ Property](dotnetimages/Property.gif) | [RotationAngle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~RotationAngle.html) | Gets or sets the angle of component rotation in this regular or radial explode step. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetComponent.html) | Gets the specified component in this explode step. |
| ![ Method](dotnetimages/Method.gif) | [GetComponentName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetComponentName.html) | Gets the name of the specified component in this explode step. |
| ![ Method](dotnetimages/Method.gif) | [GetComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetComponents.html) | Gets the components of this explode step. |
| ![ Method](dotnetimages/Method.gif) | [GetComponentXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetComponentXform.html) | Gets the transform of this explode step. |
| ![ Method](dotnetimages/Method.gif) | [GetExplodeDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetExplodeDirection.html) | Gets the explode direction (manipulator index and entity) for this explode step. |
| ![ Method](dotnetimages/Method.gif) | [GetNumOfComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetNumOfComponents.html) | Gets the number of components in this explode step. |
| ![ Method](dotnetimages/Method.gif) | [GetRotationAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetRotationAxis.html) | Gets the rotation axis (manipulator index and entity) for this regular explode step. |
| ![ Method](dotnetimages/Method.gif) | [GetSpecificComponentXForm](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetSpecificComponentXForm.html) | Gets the transformation matrix of the specified component in this explode step. |
| ![ Method](dotnetimages/Method.gif) | [GetSubAssemblyExplodeSteps](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetSubAssemblyExplodeSteps.html) | Gets the explode steps of this subassembly explode step. |
| ![ Method](dotnetimages/Method.gif) | [IGetComponent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~IGetComponent.html) | Gets the specified component in this explode step. |
| ![ Method](dotnetimages/Method.gif) | [IGetComponentXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~IGetComponentXform.html) | Gets the transform for this explode step. |
| ![ Method](dotnetimages/Method.gif) | [IsSubAssemblyRigid](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~IsSubAssemblyRigid.html) | Gets whether the subassembly is rigid or flexible. |
| ![ Method](dotnetimages/Method.gif) | [SetComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~SetComponents.html) | Specifies the components of this explode step. |
| ![ Method](dotnetimages/Method.gif) | [SetExplodeDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~SetExplodeDirection.html) | Sets the explode direction (manipulator index and entity) for this explode step. |
| ![ Method](dotnetimages/Method.gif) | [SetRotationAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~SetRotationAxis.html) | Sets the rotation axis (manipulator index and entity) for this regular explode step. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IExplodeStep Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IAssemblyDoc::ShowExploded Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ShowExploded.html)

[IModelDoc2::IsExploded Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IsExploded.html)