<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12~CreatePluginMenu2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreatePluginMenu2 Method (IEdmVault12) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault12 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12.html) : CreatePluginMenu2 Method (IEdmVault12) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hMenu*
:   Handle of menu in which to insert command items

*lInsertPosition*
:   Zero-based index of position in menu where new items are inserted; -1 to append new menu items to the bottom of the menu

*plStartID*
:   Menu command ID to assign new commands when this method is called; next available menu command ID after this method returns

*poSelObjects*
:   [IEdmSelectionList6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6.html); selected objects for which to display the menu

*lCreateMenuFlags*
:   Combination of [CreateMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.CreateMenuFlags.html) bits

*plItemCount*
:   Number of menu command items added

Inserts into a menu with the specified handle all of the menu commands registered by the SOLIDWORKS PDM Professional add-ins.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreatePluginMenu2( _    ByVal hMenu As System.Integer, _    ByVal lInsertPosition As System.Integer, _    ByRef plStartID As System.Integer, _    ByVal poSelObjects As IEdmSelectionList6, _    ByVal lCreateMenuFlags As System.Integer, _    ByRef plItemCount As System.Integer _ ) As IEdmMenu7 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmMenu7 CreatePluginMenu2(     System.int hMenu,    System.int lInsertPosition,    out System.int plStartID,    IEdmSelectionList6 poSelObjects,    System.int lCreateMenuFlags,    out System.int plItemCount ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmMenu7^ CreatePluginMenu2(  &   System.int hMenu, &   System.int lInsertPosition, &   [Out] System.int plStartID, &   IEdmSelectionList6^ poSelObjects, &   System.int lCreateMenuFlags, &   [Out] System.int plItemCount ) ``` | |

#### Parameters

*hMenu*
:   Handle of menu in which to insert command items

*lInsertPosition*
:   Zero-based index of position in menu where new items are inserted; -1 to append new menu items to the bottom of the menu

*plStartID*
:   Menu command ID to assign new commands when this method is called; next available menu command ID after this method returns

*poSelObjects*
:   [IEdmSelectionList6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6.html); selected objects for which to display the menu

*lCreateMenuFlags*
:   Combination of [CreateMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.CreateMenuFlags.html) bits

*plItemCount*
:   Number of menu command items added

#### Return Value

[IEdmMenu7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu7.html) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Display Menu of Commands (VB.NET)](Display_Menu_of_Commands_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmVault5::CreatePluginMenu](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~CreatePluginMenu.html) by adding the ability to insert a menu for object types other than files and folders (e.g., items).

Use the returned interface to call [IEdmMenu7::OnMenuItem2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu7~OnMenuItem2.html) when the user selects one of the command items added by this method.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault12 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12.html)

[IEdmVault12 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011