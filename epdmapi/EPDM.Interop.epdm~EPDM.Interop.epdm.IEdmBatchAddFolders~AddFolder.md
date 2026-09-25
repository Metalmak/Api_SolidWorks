<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders~AddFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFolder Method (IEdmBatchAddFolders) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchAddFolders Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders.html) : AddFolder Method (IEdmBatchAddFolders) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentFolderID*
:   ID of parent folder to which to add the folders

*bsRelativePath*
:   Name of folder or relative path of new folder

*lParam*
:   Caller-defined value

*lEdmBatchAddFolderFlags*
:   Combination of [EdmBatchAddFolderFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchAddFolderFlag.html) bits

*poData*
:   Optional [IEdmFolderData5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html) permission settings and card layouts are copied to the added folders

*lSourceFolderID*
:   Optional ID of folder to copy; if not 0, permission settings and card layouts from the source folder with this lSourceFolderID are copied to the added folders

Adds a folder or a complete folder path to the batch of folders to add to the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFolder( _    ByVal lParentFolderID As System.Integer, _    ByVal bsRelativePath As System.String, _    ByVal lParam As System.Integer, _    Optional ByVal lEdmBatchAddFolderFlags As System.Integer, _    Optional ByVal poData As EdmFolderData, _    Optional ByVal lSourceFolderID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFolder(     System.int lParentFolderID,    System.string bsRelativePath,    System.int lParam,    System.int lEdmBatchAddFolderFlags,    EdmFolderData poData,    System.int lSourceFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFolder(  &   System.int lParentFolderID, &   System.String^ bsRelativePath, &   System.int lParam, &   System.int lEdmBatchAddFolderFlags, &   EdmFolderData^ poData, &   System.int lSourceFolderID ) ``` | |

#### Parameters

*lParentFolderID*
:   ID of parent folder to which to add the folders

*bsRelativePath*
:   Name of folder or relative path of new folder

*lParam*
:   Caller-defined value

*lEdmBatchAddFolderFlags*
:   Combination of [EdmBatchAddFolderFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchAddFolderFlag.html) bits

*poData*
:   Optional [IEdmFolderData5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html) permission settings and card layouts are copied to the added folders

*lSourceFolderID*
:   Optional ID of folder to copy; if not 0, permission settings and card layouts from the source folder with this lSourceFolderID are copied to the added folders

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchAddFolders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, you must call [IEdmBatchAddFolders::Create](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders~Create.html) to actually add the folder to the vault.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_NAME: The folder name contained invalid characters.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchAddFolders Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders.html)

[IEdmBatchAddFolders Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional