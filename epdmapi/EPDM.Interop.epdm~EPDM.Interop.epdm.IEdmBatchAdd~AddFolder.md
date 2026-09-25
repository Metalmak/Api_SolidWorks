<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~AddFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFolder Method (IEdmBatchAdd) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchAdd Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) : AddFolder Method (IEdmBatchAdd) |

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

*lArg*
:   Caller-defined argument

*lEdmBatchAddFolderFlags*
:   Combination of [EdmBatchAddFolderFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchAddFolderFlag.html) bits

*poData*
:   Optional [IEdmFolderData5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html); extra information about the folder to create

*lSourceFolderID*
:   Optional ID of source folder from which to copy properties from

Adds the specified folder or folder path to the batch of folders to be added to the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFolder( _    ByVal lParentFolderID As System.Integer, _    ByVal bsRelativePath As System.String, _    ByVal lArg As System.Integer, _    Optional ByVal lEdmBatchAddFolderFlags As System.Integer, _    Optional ByVal poData As EdmFolderData, _    Optional ByVal lSourceFolderID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFolder(     System.int lParentFolderID,    System.string bsRelativePath,    System.int lArg,    System.int lEdmBatchAddFolderFlags,    EdmFolderData poData,    System.int lSourceFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFolder(  &   System.int lParentFolderID, &   System.String^ bsRelativePath, &   System.int lArg, &   System.int lEdmBatchAddFolderFlags, &   EdmFolderData^ poData, &   System.int lSourceFolderID ) ``` | |

#### Parameters

*lParentFolderID*
:   ID of parent folder to which to add the folders

*bsRelativePath*
:   Name of folder or relative path of new folder

*lArg*
:   Caller-defined argument

*lEdmBatchAddFolderFlags*
:   Combination of [EdmBatchAddFolderFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchAddFolderFlag.html) bits

*poData*
:   Optional [IEdmFolderData5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html); extra information about the folder to create

*lSourceFolderID*
:   Optional ID of source folder from which to copy properties from

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, use [IEdmBatchAdd::SetFileNameSerNo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~SetFileNameSerNo.html) to specify how to create the name for the new file's data card.

After calling this method, you must call [IEdmBatchAdd::CommitAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~CommitAdd.html) to actually add the file to the vault.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchAdd Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html)

[IEdmBatchAdd Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional