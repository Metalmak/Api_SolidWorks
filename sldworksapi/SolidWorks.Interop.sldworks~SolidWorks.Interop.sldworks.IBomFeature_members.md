<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IBomFeature Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IBomFeature Interface |

The following tables list the members exposed by [IBomFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Configuration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~Configuration.html) | Gets or sets the name of configuration for this BOM table. |
| ![ Property](dotnetimages/Property.gif) | [DetailedCutList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~DetailedCutList.html) | Gets or sets whether to show the detailed cut list in this BOM table. |
| ![ Property](dotnetimages/Property.gif) | [DisplayAsOneItem](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~DisplayAsOneItem.html) | Gets or sets whether all of the configurations appear with the same item number if the BOM table contains components that have multiple configurations. |
| ![ Property](dotnetimages/Property.gif) | [FollowAssemblyOrder2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~FollowAssemblyOrder2.html) | Gets or sets whether the order of the item numbers in the BOM follows the order in which the assembly appears in the FeatureManager design tree. |
| ![ Property](dotnetimages/Property.gif) | [KeepCurrentItemNumbers](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~KeepCurrentItemNumbers.html) | Gets or sets whether item numbers are kept with their components when reordering rows of a BOM table. |
| ![ Property](dotnetimages/Property.gif) | [KeepMissingItems](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~KeepMissingItems.html) | Gets and sets the Keep Missing Items option for this BOM feature. |
| ![ Property](dotnetimages/Property.gif) | [KeepReplacedCompOption](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~KeepReplacedCompOption.html) | Gets or sets how to replace components when keeping missing items. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~Name.html) | Gets the name of this BOM table feature. |
| ![ Property](dotnetimages/Property.gif) | [NumberingTypeOnIndentedBOM](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~NumberingTypeOnIndentedBOM.html) | Gets and sets the type of numbering for this indented BOM table. |
| ![ Property](dotnetimages/Property.gif) | [PartConfigurationGrouping](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~PartConfigurationGrouping.html) | Gets and sets the part configuration grouping for this BOM table. |
| ![ Property](dotnetimages/Property.gif) | [RoutingComponentGrouping](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~RoutingComponentGrouping.html) | Gets or sets the routing component grouping options for this BOM table in a drawing of an assembly containing routing components. |
| ![ Property](dotnetimages/Property.gif) | [SequenceStartNumber](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~SequenceStartNumber.html) | Gets or sets the number with which to start the numbering for this BOM table. |
| ![ Property](dotnetimages/Property.gif) | [StrikeoutMissingItems](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~StrikeoutMissingItems.html) | Inserts a horizontal line through missing items in this BOM table (also called strike outs). |
| ![ Property](dotnetimages/Property.gif) | [TableType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~TableType.html) | Gets and sets the type of table for the Bill of Materials. |
| ![ Property](dotnetimages/Property.gif) | [ZeroQuantityDisplay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~ZeroQuantityDisplay.html) | Gets or sets the character or value to display when a value is 0 in this BOM table. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [FollowAssemblyOrder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~FollowAssemblyOrder.html) | Obsolete. Superseded by [IBomFeature::FollowAssemblyOrder2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature~FollowAssemblyOrder2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetConfigurationCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~GetConfigurationCount.html) | Gets the number of configurations available to this BOM table or used in this BOM table. |
| ![ Method](dotnetimages/Method.gif) | [GetConfigurations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~GetConfigurations.html) | Gets the configurations available to this BOM table or used in this BOM table. |
| ![ Method](dotnetimages/Method.gif) | [GetFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~GetFeature.html) | Gets the BOM table feature. |
| ![ Method](dotnetimages/Method.gif) | [GetReferencedModelName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~GetReferencedModelName.html) | Gets the name of the model referenced by this BOM feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTableAnnotationCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~GetTableAnnotationCount.html) | Gets the number of BOM table annotations for this BOM table feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTableAnnotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~GetTableAnnotations.html) | Gets the BOM table annotations for this BOM table feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetConfigurations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~IGetConfigurations.html) | Gets the configurations available to this BOM table or used in this BOM table. |
| ![ Method](dotnetimages/Method.gif) | [IGetTableAnnotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~IGetTableAnnotations.html) | Gets the BOM table annotations for this BOM table feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetConfigurations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~ISetConfigurations.html) | Sets the configurations used in this BOM table. |
| ![ Method](dotnetimages/Method.gif) | [SetConfigurations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~SetConfigurations.html) | Sets the configurations used in this BOM table. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IBomFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)