<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWShell Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWShell Interface |

The following tables list the members exposed by [ICWShell](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CompositeOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~CompositeOptions.html) | Gets the options for this composite shell. |
| ![ Property](dotnetimages/Property.gif) | [EntityCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~EntityCount.html) | Gets the number of entities in the shell. |
| ![ Property](dotnetimages/Property.gif) | [Formulation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~Formulation.html) | Gets or sets the formulation type for the shell. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~Name.html) | Gets the name of the shell. |
| ![ Property](dotnetimages/Property.gif) | [ShellOffsetOption](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~ShellOffsetOption.html) | Gets or sets the shell offset option. |
| ![ Property](dotnetimages/Property.gif) | [ShellOffsetValue](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~ShellOffsetValue.html) | Gets or sets the shell offset value. |
| ![ Property](dotnetimages/Property.gif) | [ShellThickness](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~ShellThickness.html) | Gets or sets the shell thickness. |
| ![ Property](dotnetimages/Property.gif) | [ShellUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~ShellUnit.html) | Gets or sets the units for the shell thickness. |
| ![ Property](dotnetimages/Property.gif) | [State](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~State.html) | Gets the state of suppression of the shell. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetDefaultMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~GetDefaultMaterial.html) | Gets the CAD material of the shell. |
| ![ Method](dotnetimages/Method.gif) | [GetDisplayName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~GetDisplayName.html) | Gets the name of this shell as displayed in the Simulation tree. |
| ![ Method](dotnetimages/Method.gif) | [GetEntityAt](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~GetEntityAt.html) | Gets the entity at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [GetShellMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~GetShellMaterial.html) | Gets the material applied to the shell for analysis. |
| ![ Method](dotnetimages/Method.gif) | [InsertEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~InsertEntity.html) | Inserts an entity. |
| ![ Method](dotnetimages/Method.gif) | [RemoveEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~RemoveEntity.html) | Removes the entity at the specified index from the shell. |
| ![ Method](dotnetimages/Method.gif) | [SetFavMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetFavMaterial.html) | Obsolete. Superseded by [ICWShell::SetFavMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetFavMaterial2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetFavMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetFavMaterial2.html) | Applies the specified material from the material favorites list. |
| ![ Method](dotnetimages/Method.gif) | [SetLibraryMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetLibraryMaterial.html) | Obsolete. Superseded by [ICWShell::SetLibraryMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetLibraryMaterial2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetLibraryMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetLibraryMaterial2.html) | Sets the material library and material name for the shell. |
| ![ Method](dotnetimages/Method.gif) | [SetShellMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetShellMaterial.html) | Sets the material to apply to the shell for analysis. |
| ![ Method](dotnetimages/Method.gif) | [ShellBeginEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~ShellBeginEdit.html) | Starts editing the shell. |
| ![ Method](dotnetimages/Method.gif) | [ShellEndEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~ShellEndEdit.html) | Ends editing a shell. |
| ![ Method](dotnetimages/Method.gif) | [SuppressUnSuppress](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SuppressUnSuppress.html) | Suppresses or unsuppresses the shell depending on its [state](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWShell~State.html). |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWShell Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWShellManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager.html)

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)