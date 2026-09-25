<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveFromMenu.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RemoveFromMenu Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RemoveFromMenu Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommandID*
:   Command ID of the command to remove as defined by swCommands\_e

*DocumentType*
:   Document types in which to remove the command as defined in swDocumentTypes\_e

*Option*
:   * 1 = Menu

      * 2 = Toolbar

        * 3 = Both menu and toolbar

*RemoveParentMenu*
:   True to remove the specified command's parent menu, false to not

    NOTE: This parameter is specific to menus only; it does not affect toolbars.

Removes:

* the specified command from all main frame menus or a toolbar or both

  * the specified command's parent menus

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RemoveFromMenu( _    ByVal CommandID As System.Integer, _    ByVal DocumentType As System.Integer, _    ByVal Option As System.Integer, _    ByVal RemoveParentMenu As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim CommandID As System.Integer Dim DocumentType As System.Integer Dim Option As System.Integer Dim RemoveParentMenu As System.Boolean Dim value As System.Boolean   value = instance.RemoveFromMenu(CommandID, DocumentType, Option, RemoveParentMenu) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RemoveFromMenu(     System.int CommandID,    System.int DocumentType,    System.int Option,    System.bool RemoveParentMenu ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RemoveFromMenu(  &   System.int CommandID, &   System.int DocumentType, &   System.int Option, &   System.bool RemoveParentMenu ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CommandID*
:   Command ID of the command to remove as defined by swCommands\_e

*DocumentType*
:   Document types in which to remove the command as defined in swDocumentTypes\_e

*Option*
:   * 1 = Menu

      * 2 = Toolbar

        * 3 = Both menu and toolbar

*RemoveParentMenu*
:   True to remove the specified command's parent menu, false to not

    NOTE: This parameter is specific to menus only; it does not affect toolbars.

#### Return Value

True if the specified items are removed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::RemoveFromMenu.

# ![](dotnetimages/collapse.gif)Example

[Remove Menu Commands, Menus, and Toolbar Buttons (VBA)](Remove_Menu_Commands_Menus_and_Toolbar_Buttons_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method does not affect context-sensitive menus (also called shortcut menus and pop-up menus); this command only affects main frame menus and toolbars. To remove commands and parent menus from context-sensitive menus, use [ISldWorks::RemoveFromPopupMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RemoveFromPopupMenu.html).

The specified items are removed after this method executes, and their removal can be seen immediately.

This method is not persistent across SOLIDWORKS sessions.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenu.html)

[ISldWorks::AddMenuItem3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuItem3.html)

[ISldWorks::AddMenuPopupItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuPopupItem2.html)

[ISldWorks::AddToolbar4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbar4.html)

[ISldWorks::AddToolbarCommand2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbarCommand2.html)

[ISldWorks::DragToolbarButton Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~DragToolbarButton.html)

[ISldWorks::HideToolbar2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~HideToolbar2.html)

[ISldWorks::RemoveMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveMenu.html)

[ISldWorks::RemoveMenuPopupItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveMenuPopupItem2.html)

[ISldWorks::RemoveToolbar2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveToolbar2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP2, Revision Number 15.2