<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWBearingLoad Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWBearingLoad Interface |

The following tables list the members exposed by [ICWBearingLoad](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [BearingLoadUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~BearingLoadUnit.html) | Gets or sets the unit system for this bearing load. |
| ![ Property](dotnetimages/Property.gif) | [Direction](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~Direction.html) | Gets or sets the direction of this bearing load in the selected coordinate system. |
| ![ Property](dotnetimages/Property.gif) | [DistributionType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~DistributionType.html) | Gets or sets the distribution type of this bearing load. |
| ![ Property](dotnetimages/Property.gif) | [UseTimeCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~UseTimeCurve.html) | Obsolete. Superseded by [ICWBearingLoad::UseTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~UseTimeCurve2.html). |
| ![ Property](dotnetimages/Property.gif) | [UseTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~UseTimeCurve2.html) | Gets or sets whether to use a time curve for this bearing load. |
| ![ Property](dotnetimages/Property.gif) | [XDirectionReverse](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~XDirectionReverse.html) | Obsolete. Superseded by [ICWBearingLoad::XDirectionReverse2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~XDirectionReverse2.html). |
| ![ Property](dotnetimages/Property.gif) | [XDirectionReverse2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~XDirectionReverse2.html) | Gets or sets whether to reverse the X direction of this bearing load. |
| ![ Property](dotnetimages/Property.gif) | [XDirectionValue](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~XDirectionValue.html) | Gets or sets the value of the bearing load in the X direction of the selected coordinate system. |
| ![ Property](dotnetimages/Property.gif) | [YDirectionReverse](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~YDirectionReverse.html) | Obsolete. Superseded by [ICWBearingLoad::YDirectionReverse2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~YDirectionReverse2.html). |
| ![ Property](dotnetimages/Property.gif) | [YDirectionReverse2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~YDirectionReverse2.html) | Gets or sets whether to reverse the Y direction of this bearing load. |
| ![ Property](dotnetimages/Property.gif) | [YDirectionValue](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~YDirectionValue.html) | Gets or sets the value of the bearing load in the Y direction of the selected coordinate system. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [BearingLoadBeginEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~BearingLoadBeginEdit.html) | Starts editing a bearing load. |
| ![ Method](dotnetimages/Method.gif) | [BearingLoadEndEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~BearingLoadEndEdit.html) | Ends editing a bearing load. |
| ![ Method](dotnetimages/Method.gif) | [GetEntityCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~GetEntityCount.html) | Gets the number of entities for the bearing load. |
| ![ Method](dotnetimages/Method.gif) | [GetTimeCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~GetTimeCurve.html) | Gets the time curve data for the bearing load of this dynamic study. |
| ![ Method](dotnetimages/Method.gif) | [InsertEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~InsertEntity.html) | Inserts a source entity for the bearing load. |
| ![ Method](dotnetimages/Method.gif) | [RemoveEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~RemoveEntity.html) | Removes a source entity at the specified index from the bearing load. |
| ![ Method](dotnetimages/Method.gif) | [ReplaceCoordinateSystem](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~ReplaceCoordinateSystem.html) | Replace the current coordinate system with the specified coordinate system. |
| ![ Method](dotnetimages/Method.gif) | [SetTimeCurve](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~SetTimeCurve.html) | Obsolete. Superseded by [ICWBearingLoad::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~SetTimeCurve2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~SetTimeCurve2.html) | Defines a time curve for the bearing load of this dynamic study. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBearingLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)