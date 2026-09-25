<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICommandGroup Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ICommandGroup Interface |

The following tables list the members exposed by [ICommandGroup](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CommandID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~CommandID.html) | Gets the command ID for the specified item in the CommandGroup. |
| ![ Property](dotnetimages/Property.gif) | [CustomNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~CustomNames.html) | Gets or sets the custom names in the CommandGroup. |
| ![ Property](dotnetimages/Property.gif) | [DockingState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~DockingState.html) | Gets or sets the docking state of the toolbar in the CommandGroup. |
| ![ Property](dotnetimages/Property.gif) | [HasEnabledButton](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~HasEnabledButton.html) | Gets whether any buttons in this CommandGroup are enabled. |
| ![ Property](dotnetimages/Property.gif) | [HasMenu](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~HasMenu.html) | Gets or sets whether this CommandGroup has a menu. |
| ![ Property](dotnetimages/Property.gif) | [HasToolbar](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~HasToolbar.html) | Gets or sets whether this CommandGroup has a toolbar. |
| ![ Property](dotnetimages/Property.gif) | [IconList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~IconList.html) | Gets or sets the paths for the icons for the toolbar buttons and separators for this CommandGroup. |
| ![ Property](dotnetimages/Property.gif) | [LargeIconList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~LargeIconList.html) | Obsolete. Superseded by [ICommandGroup::IconList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~IconList.html). |
| ![ Property](dotnetimages/Property.gif) | [LargeMainIcon](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~LargeMainIcon.html) | Obsolete. Superseded by [ICommandGroup::MainIconList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~MainIconList.html). |
| ![ Property](dotnetimages/Property.gif) | [MainIconList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~MainIconList.html) | Gets or sets the paths for the icons for the buttons for this CommandGroup. |
| ![ Property](dotnetimages/Property.gif) | [MenuPosition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~MenuPosition.html) | Gets or sets the position of the CommandGroup for the specified document templates. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~Name.html) | Gets the name of the CommandGroup. |
| ![ Property](dotnetimages/Property.gif) | [NumberOfGroupItems](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~NumberOfGroupItems.html) | Gets the number of items in the CommandGroup. |
| ![ Property](dotnetimages/Property.gif) | [SelectType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~SelectType.html) | This property:   * gets the type of object selected on the context sensitive, pop-up menu.* sets the type of object that the user must select to show the context sensitive, pop-up menu. |
| ![ Property](dotnetimages/Property.gif) | [ShowInDocumentType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~ShowInDocumentType.html) | Gets or sets the types of documents to show this CommandGroup. |
| ![ Property](dotnetimages/Property.gif) | [SmallIconList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~SmallIconList.html) | Obsolete. Superseded by [ICommandGroup::IconList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~IconList.html). |
| ![ Property](dotnetimages/Property.gif) | [SmallMainIcon](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~SmallMainIcon.html) | Obsolete. Superseded by [ICommandGroup::MainIconList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~MainIconList.html). |
| ![ Property](dotnetimages/Property.gif) | [ToolbarId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~ToolbarId.html) | Gets the toolbar ID of this CommandGroup. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [Activate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~Activate.html) | Activates the CommandGroup. |
| ![ Method](dotnetimages/Method.gif) | [AddCommandItem](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~AddCommandItem.html) | Obsolete. Superseded by [ICommandGroup::AddComandItem2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~AddCommandItem2.html). |
| ![ Method](dotnetimages/Method.gif) | [AddCommandItem2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~AddCommandItem2.html) | Adds a combination menu item and toolbar item to a CommandGroup. |
| ![ Method](dotnetimages/Method.gif) | [AddSpacer](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~AddSpacer.html) | Obsolete. Superseded by [ICommandGroup::AddSpacer2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~AddSpacer2.html). |
| ![ Method](dotnetimages/Method.gif) | [AddSpacer2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~AddSpacer2.html) | Adds a spacer between items in a CommandGroup. |
| ![ Method](dotnetimages/Method.gif) | [GetToolbarVisibility](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~GetToolbarVisibility.html) | Gets whether this toolbar is visible. |
| ![ Method](dotnetimages/Method.gif) | [SetToolbarVisibility](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~SetToolbarVisibility.html) | Sets the visibility of the toolbar in the CommandGroup. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICommandGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)