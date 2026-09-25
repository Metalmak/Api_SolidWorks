<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IConfigurationManager Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IConfigurationManager Interface |

The following tables list the members exposed by [IConfigurationManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [ActiveConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ActiveConfiguration.html) | Gets the active configuration. |
| ![ Property](dotnetimages/Property.gif) | [Document](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~Document.html) | Gets the related model document. |
| ![ Property](dotnetimages/Property.gif) | [EnableConfigurationTree](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~EnableConfigurationTree.html) | Gets or sets whether to update the ConfigurationManager tree. |
| ![ Property](dotnetimages/Property.gif) | [LinkDisplayStatesToConfigurations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~LinkDisplayStatesToConfigurations.html) | Gets or sets whether to link or unlink display states to or from the active configuration. |
| ![ Property](dotnetimages/Property.gif) | [ShowConfigurationDescriptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ShowConfigurationDescriptions.html) | Gets or sets whether to display configuration descriptions in ConfigurationManager. |
| ![ Property](dotnetimages/Property.gif) | [ShowConfigurationNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ShowConfigurationNames.html) | Gets or sets whether to display configuration names in ConfigurationManager. |
| ![ Property](dotnetimages/Property.gif) | [ShowPreview](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ShowPreview.html) | Gets or sets whether to display the preview of a selected configuration. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddCADFamilyConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddCADFamilyConfiguration.html) | Adds the specified configuration to SOLIDWORKS Connected. |
| ![ Method](dotnetimages/Method.gif) | [AddConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddConfiguration.html) | Obsolete. Superseded by [IConfigurationManager::AddConfiguration2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddConfiguration2.html). |
| ![ Method](dotnetimages/Method.gif) | [AddConfiguration2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddConfiguration2.html) | Creates a new configuration. |
| ![ Method](dotnetimages/Method.gif) | [AddRebuildSaveMark](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddRebuildSaveMark.html) | Adds marks indicating whether the specified configurations need to be rebuilt and their configuration data saved every time the model document is saved. |
| ![ Method](dotnetimages/Method.gif) | [AddSpeedPak](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddSpeedPak.html) | Obsolete. Superseded by [IConfigurationManager::AddSpeedPak2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfigurationManager~AddSpeedPak2.html). |
| ![ Method](dotnetimages/Method.gif) | [AddSpeedPak2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddSpeedPak2.html) | Creates a SpeedPak configuration that includes all faces and the specified threshold of parts or bodies for the active assembly configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetConfigurationParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~GetConfigurationParams.html) | Gets the parameters for this configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetConfigurationParamsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~GetConfigurationParamsCount.html) | Gets the number of parameters for this configuration. |
| ![ Method](dotnetimages/Method.gif) | [IGetConfigurationParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~IGetConfigurationParams.html) | Gets the parameters for this configuration. |
| ![ Method](dotnetimages/Method.gif) | [ISetConfigurationParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ISetConfigurationParams.html) | Sets the parameters for this configuration. |
| ![ Method](dotnetimages/Method.gif) | [RemoveMarkForAllConfigurations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~RemoveMarkForAllConfigurations.html) | Remove all marks indicating whether configurations need to be rebuilt and their configuration data saved every time the model document is saved. |
| ![ Method](dotnetimages/Method.gif) | [SetConfigurationParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~SetConfigurationParams.html) | Sets the parameters for this configuration. |
| ![ Method](dotnetimages/Method.gif) | [SetExpanded](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~SetExpanded.html) | Sets whether to display and expand all of the configuration nodes in the specified pane of the ConfigurationManager. |
| ![ Method](dotnetimages/Method.gif) | [SortConfigurationTree](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~SortConfigurationTree.html) | Specifies the order in which to list configurations in the ConfigurationManager. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)