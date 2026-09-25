<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~CreatePluginMenu.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreatePluginMenu Method (IEdmVault5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : CreatePluginMenu Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hMenu*
:   Handle of menu in which to insert add-in commands

*lInsertPosition*
:   Zero-based index of the position in the menu where new menu items should be inserted; -1 to append new menu items to the bottom of the menu

*plStartID*
:   Next available menu command ID (see **Remarks**)

*lSelFileCount*
:   Number of selected files

*lSelFolderCount*
:   Number of selected folders

*lCreateMenuFlags*
:   Combination of [CreateMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.CreateMenuFlags.html) bits

*plItemCount*
:   Number of menu items added

Obsolete. Superseded by [IEdmVault12::CreatePluginMenu2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12~CreatePluginMenu2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreatePluginMenu( _    ByVal hMenu As System.Integer, _    ByVal lInsertPosition As System.Integer, _    ByRef plStartID As System.Integer, _    ByVal lSelFileCount As System.Integer, _    ByVal lSelFolderCount As System.Integer, _    ByVal lCreateMenuFlags As System.Integer, _    ByRef plItemCount As System.Integer _ ) As IEdmMenu5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmMenu5 CreatePluginMenu(     System.int hMenu,    System.int lInsertPosition,    out System.int plStartID,    System.int lSelFileCount,    System.int lSelFolderCount,    System.int lCreateMenuFlags,    out System.int plItemCount ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmMenu5^ CreatePluginMenu(  &   System.int hMenu, &   System.int lInsertPosition, &   [Out] System.int plStartID, &   System.int lSelFileCount, &   System.int lSelFolderCount, &   System.int lCreateMenuFlags, &   [Out] System.int plItemCount ) ``` | |

#### Parameters

*hMenu*
:   Handle of menu in which to insert add-in commands

*lInsertPosition*
:   Zero-based index of the position in the menu where new menu items should be inserted; -1 to append new menu items to the bottom of the menu

*plStartID*
:   Next available menu command ID (see **Remarks**)

*lSelFileCount*
:   Number of selected files

*lSelFolderCount*
:   Number of selected folders

*lCreateMenuFlags*
:   Combination of [CreateMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.CreateMenuFlags.html) bits

*plItemCount*
:   Number of menu items added

#### Return Value

[IEdmMenu5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

# ![](dotnetimages/collapse.gif)Remarks

When this method is called, plStartID should be the first free menu command ID that a new command is assigned. When this method returns, plStartID is the first free menu command ID after IDs for new menu commands have been reserved.

When the user chooses one of the menu items added by this method, your program must call [IEdmMenu5::OnMenuItem](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~OnMenuItem.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2