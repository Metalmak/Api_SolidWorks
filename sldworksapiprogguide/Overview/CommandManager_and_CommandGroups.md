<!-- source: sldworksapiprogguide/Overview/CommandManager_and_CommandGroups.htm -->

# SOLIDWORKS API Help

# CommandManager and CommandGroups

You can create native SOLIDWORKS toolbars and menus using
ICommandManager
and ICommandGroup.

NOTE: You can only create one
CommandManager in an add-in application; however, multiple CommandGroups
can exist in an add-in application. See SOLIDWORKS Help for details about
the CommandManager.

The CommandManager-style toolbars and menus:

* Allowo you to add toolbars to the SOLIDWORKS CommandManager.
* Allow you to drag your toolbar buttons to and from other API
  and native SOLIDWORKS toolbars using the Tools,
  Customize dialog or ISldWorks::DragToolbarButton.
* Allow you to create flyout toolbars and submenus.
* Are associated, so they use the same name, button, callback function,
  enable function, and add-in ID.

You cannot create an ICommandGroup with a toolbar, start SOLIDWORKS,
use the toolbar, close SOLIDWORKS, add items to or remove items from the
toolbar, and start SOLIDWORKS. Instead, to add to or remove items from a
toolbar during development, you must:

1. Call
   ICommandGroup::ToolbarId
   to get the ID of the toolbar you want to modify.
2. Use the ID to find the toolbar in the registry.
3. Remove the toolbar definition
   from the registry:
   HKEY\_CURRENT\_USER\Software\SOLIDWORKS\SOLIDWORKS
   <version>\User Interface\Custom API Toolbars\<index>
   HKEY\_CURRENT\_USER\Software\SOLIDWORKS\SOLIDWORKS
   <version>\User Interface\Toolbars
   HKEY\_CURRENT\_USER\Software\SOLIDWORKS\SOLIDWORKS
   <version>\User Interface\Toolbars\PartTool
   HKEY\_CURRENT\_USER\Software\SOLIDWORKS\SOLIDWORKS
   <version>\User Interface\Toolbars\AssemblyTool
   HKEY\_CURRENT\_USER\Software\SOLIDWORKS\SOLIDWORKS
   <version>\User Interface\Toolbars\DrawingTool
4. Add items to and remove items from the toolbar.
5. Assign the ICommandGroup a different user ID. This is the ID generated
   by
   ICommandManager::CreateCommandGroup.
   You must keep track of the toolbar user IDs in each version of
   your add-in. The user ID and the GUID of the CoClass implementing ISwAddin
   are a unique pair.

### To add commands:

1. Create the ICommandManager using ISldWorks::GetCommandManager.

   NOTE: You might want to declare this object as a class variable
   in your add-in so that it can be accessed from anywhere later.
2. Create one or more top-level CommandGroups using
   ICommandManager::CreateCommandGroup
   or ICommandManager::AddContextMenu.
3. Add bitmap files of the images of buttons to the
   CommandGroups using ICommandGroup::LargeIconList,
   ICommandGroup::SmallIconList,
   ICommandGroup::LargeMainIcon,
   and ICommandGroup::SmallMainIcon.

   NOTE: You only add the bitmap files to the top-level group.
   These files provide the images of the buttons for all of the CommandGroups.
4. Add commands to the CommandGroups using ICommandGroup::AddCommandItem2.
5. Enable or disable toolbars or menus for specific
   CommandGroups using ICommandGroup::HasToolbar
   and ICommandGroup::HasMenu.
6. Create context-sensitive menus using ICommandGroup::SelectType
   and ICommandGroup::CustomNames,
   if the selected object is a custom feature such as an attribute.
7. Activate the top-level ICommandGroup using ICommandGroup::Activate.

### To remove commands:

Use ICommandManager::RemoveCommandGroup
for all CommandGroups created with ICommandManager::CreateCommandGroup
and ICommandManager::AddContextMenu.