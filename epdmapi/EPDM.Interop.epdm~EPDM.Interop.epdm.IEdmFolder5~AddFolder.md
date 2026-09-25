<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFolder Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : AddFolder Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*bsFolderName*
:   Name of the new folder

*poData*
:   [IEdmFolderData5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html); optional additional data (see **Remarks**)

Creates a subfolder in this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function AddFolder( _    ByVal lParentWnd As System.Integer, _    ByVal bsFolderName As System.String, _    Optional ByVal poData As EdmFolderData _ ) As IEdmFolder5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmFolder5 AddFolder(     System.int lParentWnd,    System.string bsFolderName,    EdmFolderData poData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmFolder5^ AddFolder(  &   System.int lParentWnd, &   System.String^ bsFolderName, &   EdmFolderData^ poData ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*bsFolderName*
:   Name of the new folder

*poData*
:   [IEdmFolderData5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html); optional additional data (see **Remarks**)

#### Return Value

[IEdmFolder5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

# ![](dotnetimages/collapse.gif)Example

[Add Folder (VB.NET)](Add_Folder_Example_VBNET.htm)

[Add Folder (C#)](Add_Folder_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To create all the folders in a path in one operation, call  [IEdmFolder5::CreateFolderPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateFolderPath.html).

To add more than one folder, use [IEdmBatchAddFolders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders.html) to add them all at once, which is much more efficient than using this method, which adds folders only one at a time.

If poData is null, the user rights and file data card for the new folder are inherited from the parent folder.

C++ users not using smart-pointer wrapper functions must release the returned pointer to IEdmFolder5.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_NAME: The folder name contained invalid characters.* E\_EDM\_COULD\_NOT\_CREATE\_LOCAL\_FOLDER: Could not create the new folder in the local disk cache.* E\_EDM\_NAME\_ALREADY\_EXISTS: There is already a file or folder with the specified name in this folder.* E\_EDM\_FOLDER\_NOT\_FOUND: This folder has been deleted.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to create sub-folders here.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: The operation was not permitted by one of the installed [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html).EdmCmd\_PreAddFolder hooks.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

[IEdmFolder5::CreateFolderPath Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateFolderPath.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2