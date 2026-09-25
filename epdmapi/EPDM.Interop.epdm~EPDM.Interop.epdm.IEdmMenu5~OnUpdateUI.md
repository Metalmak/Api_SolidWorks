<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~OnUpdateUI.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| OnUpdateUI Method (IEdmMenu5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html) : OnUpdateUI Method (IEdmMenu5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lSelFileCount*
:   Number of selected files

*lSelFolderCount*
:   Number of selected folders

*bAllItemsInSameFolder*
:   True if all of the selected files and folders are located in the same parent folder, false if not

Updates the menu based on a new selection of files and folders.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub OnUpdateUI( _    ByVal lSelFileCount As System.Integer, _    ByVal lSelFolderCount As System.Integer, _    Optional ByVal bAllItemsInSameFolder As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void OnUpdateUI(     System.int lSelFileCount,    System.int lSelFolderCount,    System.bool bAllItemsInSameFolder ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnUpdateUI(  &   System.int lSelFileCount, &   System.int lSelFolderCount, &   System.bool bAllItemsInSameFolder ) ``` | |

#### Parameters

*lSelFileCount*
:   Number of selected files

*lSelFolderCount*
:   Number of selected folders

*bAllItemsInSameFolder*
:   True if all of the selected files and folders are located in the same parent folder, false if not

# ![](dotnetimages/collapse.gif)Remarks

Some items in the menu might be grayed out or removed due to the currently selected number of files and folders. This method updates the menu based on a new selection of files and folders.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html)

[IEdmMenu5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional