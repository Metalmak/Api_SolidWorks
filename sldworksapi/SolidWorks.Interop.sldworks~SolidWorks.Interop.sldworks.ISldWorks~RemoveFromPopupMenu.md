<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveFromPopupMenu.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RemoveFromPopupMenu Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RemoveFromPopupMenu Method (ISldWorks) |

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

*SelectionType*
:   Context-sensitive menu from which to remove the command as defined by swSelectType\_e

    NOTE: Specifying swSelEVERYTHING will remove the command from all context-sensitive menus

*RemoveParentMenu*
:   True to remove the specified command's any parent menus, false to not

Removes the specified menu item from one or all specified context-sensitive menus (also called shortcut menus and pop-up menus) for the specified document types.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RemoveFromPopupMenu( _    ByVal CommandID As System.Integer, _    ByVal DocumentType As System.Integer, _    ByVal SelectionType As System.Integer, _    ByVal RemoveParentMenu As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim CommandID As System.Integer Dim DocumentType As System.Integer Dim SelectionType As System.Integer Dim RemoveParentMenu As System.Boolean Dim value As System.Boolean   value = instance.RemoveFromPopupMenu(CommandID, DocumentType, SelectionType, RemoveParentMenu) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RemoveFromPopupMenu(     System.int CommandID,    System.int DocumentType,    System.int SelectionType,    System.bool RemoveParentMenu ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RemoveFromPopupMenu(  &   System.int CommandID, &   System.int DocumentType, &   System.int SelectionType, &   System.bool RemoveParentMenu ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CommandID*
:   Command ID of the command to remove as defined by swCommands\_e

*DocumentType*
:   Document types in which to remove the command as defined in swDocumentTypes\_e

*SelectionType*
:   Context-sensitive menu from which to remove the command as defined by swSelectType\_e

    NOTE: Specifying swSelEVERYTHING will remove the command from all context-sensitive menus

*RemoveParentMenu*
:   True to remove the specified command's any parent menus, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::RemoveFromPopupMenu.

# ![](dotnetimages/collapse.gif)Example

[Remove Menu commands, Menus, and Toolbar Buttons (VBA)](Remove_Menu_Commands_Menus_and_Toolbar_Buttons_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The removal of the specified menu item takes affect the next time the context-sensitive menu is displayed.

To remove main frame menu commands and menus, use [ISldWorks::RemoveFromMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RemoveFromMenu.html).

This method is not persistent across SOLIDWORKS sessions.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenu.html)

[ISldWorks::AddMenuItem3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuItem3.html)

[ISldWorks::AddMenuPopupItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuPopupItem2.html)

[ISldWorks::RemoveMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveMenu.html)

[ISldWorks::RemoveMenuPopupItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveMenuPopupItem2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP2, Revision Number 15.2