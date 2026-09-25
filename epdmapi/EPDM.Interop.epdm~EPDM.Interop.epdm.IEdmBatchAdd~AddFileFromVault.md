<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~AddFileFromVault.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFileFromVault Method (IEdmBatchAdd) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchAdd Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) : AddFileFromVault Method (IEdmBatchAdd) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lSourceFileID*
:   ID of file to copy

*lSourceFolderID*
:   ID of folder of file to copy

*lDestinationFolderID*
:   ID of folder to which to copy the file

*lArg*
:   Caller-defined argument.

*bsNewName*
:   Optional new name of file.

*lEdmAddFlags*
:   Combination of [EdmAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFlag.html) bits

Adds a file with the specified ID and folder ID to the batch of files to be added to the vault; the file will be copied to a new vault folder with the specified ID.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFileFromVault( _    ByVal lSourceFileID As System.Integer, _    ByVal lSourceFolderID As System.Integer, _    ByVal lDestinationFolderID As System.Integer, _    Optional ByVal lArg As System.Integer, _    Optional ByVal bsNewName As System.String, _    Optional ByVal lEdmAddFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFileFromVault(     System.int lSourceFileID,    System.int lSourceFolderID,    System.int lDestinationFolderID,    System.int lArg,    System.string bsNewName,    System.int lEdmAddFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFileFromVault(  &   System.int lSourceFileID, &   System.int lSourceFolderID, &   System.int lDestinationFolderID, &   System.int lArg, &   System.String^ bsNewName, &   System.int lEdmAddFlags ) ``` | |

#### Parameters

*lSourceFileID*
:   ID of file to copy

*lSourceFolderID*
:   ID of folder of file to copy

*lDestinationFolderID*
:   ID of folder to which to copy the file

*lArg*
:   Caller-defined argument.

*bsNewName*
:   Optional new name of file.

*lEdmAddFlags*
:   Combination of [EdmAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFlag.html) bits

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