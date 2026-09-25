<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICommandManager Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ICommandManager Interface |

The following tables list the members exposed by [ICommandManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [NumberOfFlyoutGroups](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~NumberOfFlyoutGroups.html) | Gets the number of flyouts in the CommandManager. |
| ![ Property](dotnetimages/Property.gif) | [NumberOfGroups](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~NumberOfGroups.html) | Gets the number of CommandGroups. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddCommandTab](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~AddCommandTab.html) | Adds a tab to the CommandManager for the specified document type. |
| ![ Method](dotnetimages/Method.gif) | [AddContextMenu](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~AddContextMenu.html) | Adds a new context-sensitive menu to the CommandManager. |
| ![ Method](dotnetimages/Method.gif) | [CommandTabs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~CommandTabs.html) | Gets all of the add-in CommandManager tabs for the specified document type. |
| ![ Method](dotnetimages/Method.gif) | [CreateCommandGroup](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~CreateCommandGroup.html) | Obsolete. Superseded by [ICommandManager::CreateCommandGroup2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandManager~CreateCommandGroup2.html). |
| ![ Method](dotnetimages/Method.gif) | [CreateCommandGroup2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~CreateCommandGroup2.html) | Creates a new CommandGroup in the CommandManager. |
| ![ Method](dotnetimages/Method.gif) | [CreateFlyoutGroup](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~CreateFlyoutGroup.html) | Obsolete. Superseded by [ICommandManager::CreateFlyoutGroup2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~CreateFlyoutGroup2.html). |
| ![ Method](dotnetimages/Method.gif) | [CreateFlyoutGroup2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~CreateFlyoutGroup2.html) | Creates a new flyout in the CommandManager and context-sensitive menus. |
| ![ Method](dotnetimages/Method.gif) | [GetCommandGroup](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~GetCommandGroup.html) | Gets the CommandGroup using the specified ID. |
| ![ Method](dotnetimages/Method.gif) | [GetCommandIDsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~GetCommandIDsCount.html) | Gets the number of command IDs for the given command group. |
| ![ Method](dotnetimages/Method.gif) | [GetCommandTab](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~GetCommandTab.html) | Gets the specified CommandManager tab for the specified document type. |
| ![ Method](dotnetimages/Method.gif) | [GetCommandTabCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~GetCommandTabCount.html) | Gets the number of tabs on the CommandManager for the specified document type. |
| ![ Method](dotnetimages/Method.gif) | [GetFlyoutGroup](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~GetFlyoutGroup.html) | Gets the flyout with the specified ID. |
| ![ Method](dotnetimages/Method.gif) | [GetFlyoutGroups](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~GetFlyoutGroups.html) | Gets the flyouts in the CommandManager. |
| ![ Method](dotnetimages/Method.gif) | [GetGroupDataFromRegistry](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~GetGroupDataFromRegistry.html) | Gets the command IDs of the given command group from the registry. |
| ![ Method](dotnetimages/Method.gif) | [GetGroups](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~GetGroups.html) | Gets the CommandGroups in the CommandManager. |
| ![ Method](dotnetimages/Method.gif) | [IGetCommandTabs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~IGetCommandTabs.html) | Gets the CommandManager tabs for the specified document type. |
| ![ Method](dotnetimages/Method.gif) | [IGetGroupDataFromRegistry](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~IGetGroupDataFromRegistry.html) | Gets the command IDs of the given command group from the registry. |
| ![ Method](dotnetimages/Method.gif) | [IGetGroups](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~IGetGroups.html) | Gets the CommandGroups in the CommandManager. |
| ![ Method](dotnetimages/Method.gif) | [RemoveCommandGroup](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~RemoveCommandGroup.html) | Obsolete. Superseded by [ICommandManager::RemoveCommandGroup2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandManager~RemoveCommandGroup2.html). |
| ![ Method](dotnetimages/Method.gif) | [RemoveCommandGroup2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~RemoveCommandGroup2.html) | Removes the specified CommandGroup from the CommandManager. |
| ![ Method](dotnetimages/Method.gif) | [RemoveCommandTab](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~RemoveCommandTab.html) | Removes the specified CommandManager tab, including its tab boxes and buttons, from the CommandManager. |
| ![ Method](dotnetimages/Method.gif) | [RemoveFlyoutGroup](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~RemoveFlyoutGroup.html) | Removes the specified flyout from the CommandManager. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICommandManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)