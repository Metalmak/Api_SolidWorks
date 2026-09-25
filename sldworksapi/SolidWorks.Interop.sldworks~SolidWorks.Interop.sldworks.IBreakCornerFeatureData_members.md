<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IBreakCornerFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IBreakCornerFeatureData Interface |

The following tables list the members exposed by [IBreakCornerFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [BreakType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~BreakType.html) | Gets or sets the break corner type. |
| ![ Property](dotnetimages/Property.gif) | [CenteredOnBendLines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~CenteredOnBendLines.html) | Gets or sets whether to center the corner cuts relative to the bend lines of this break corner feature. |
| ![ Property](dotnetimages/Property.gif) | [Distance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~Distance.html) | Gets or sets the chamfer length or fillet radius, depending on the break corner type. |
| ![ Property](dotnetimages/Property.gif) | [Entities](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~Entities.html) | Gets or sets the faces or edges to which this break corner is applied. |
| ![ Property](dotnetimages/Property.gif) | [InternalCornersOnly](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~InternalCornersOnly.html) | Gets or sets whether to add or subtract material from break corner/corner trim features. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~AccessSelections.html) | Gains access to the selections that describe this break corner feature. |
| ![ Method](dotnetimages/Method.gif) | [GetEntitiesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~GetEntitiesCount.html) | Gets the number of faces or edges associated with this break corner feature. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~IAccessSelections.html) | Gains access to the selections that describe this break corner feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetEntities](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~IGetEntities.html) | Gets the faces or edges to which this break corner is applied. |
| ![ Method](dotnetimages/Method.gif) | [ISetEntities](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~ISetEntities.html) | Sets the faces or edges to which this break corner is applied. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData~ReleaseSelectionAccess.html) | Releases access to selections for this break corner feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IBreakCornerFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::InsertSheetMetalCornerTrim Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSheetMetalCornerTrim.html)

[IModelDoc2::InsertSheetMetalBreakCorner Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSheetMetalBreakCorner.html)