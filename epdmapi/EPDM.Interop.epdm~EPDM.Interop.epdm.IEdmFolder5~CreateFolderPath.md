<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateFolderPath.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateFolderPath Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : CreateFolderPath Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsPath*
:   Path of subfolders to create

*lParentWnd*
:   Parent window handle

Creates all subfolders in a path relative to this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateFolderPath( _    ByVal bsPath As System.String, _    ByVal lParentWnd As System.Integer _ ) As IEdmFolder5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmFolder5 CreateFolderPath(     System.string bsPath,    System.int lParentWnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmFolder5^ CreateFolderPath(  &   System.String^ bsPath, &   System.int lParentWnd ) ``` | |

#### Parameters

*bsPath*
:   Path of subfolders to create

*lParentWnd*
:   Parent window handle

#### Return Value

IEdmFolder5; interface to the top folder

# ![](dotnetimages/collapse.gif)Example

[Add Files to Vault (VB.NET)](Add_Files_to_Vault_Example_VBNET.htm)

[Add Files to Vault (C#)](Add_Files_to_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method does not fail if one of the subfolders in bsPath already exists.

This method does not specify file data cards or user rights for the new subfolders in bsPath. Instead of calling this method, call [IEdmFolder5::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFolder.html) to create each subfolder in the path and also specify file data cards or user rights.

It is more efficient to use [IEdmBatchAddFolders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders.html) to create many folder paths at once than to use this method to create each folder path separately.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmFolder5.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_NAME: The folder name contained invalid characters.* E\_EDM\_COULD\_NOT\_CREATE\_LOCAL\_FOLDER: Could not create the new folder in the local disk cache.* E\_EDM\_FOLDER\_NOT\_FOUND: This folder has been deleted.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to create sub-folders here.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: The operation was not permitted by one of the installed [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html).EdmCmd\_PreAddFolder hooks.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2