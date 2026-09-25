<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~AddFileFromPath.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFileFromPath Method (IEdmBatchAdd) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchAdd Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) : AddFileFromPath Method (IEdmBatchAdd) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsSourcePath*
:   Path of file to add

*lDestinationFolderID*
:   ID of folder to which to add the file

*lArg*
:   Caller-defined argument

*bsNewName*
:   Optional new name of the added file

*lEdmAddFlags*
:   Combination of [EdmAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFlag.html) bits

Adds a file to the batch of files to be added to the vault; the file will be copied to a destination folder with the specified ID.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFileFromPath( _    ByVal bsSourcePath As System.String, _    ByVal lDestinationFolderID As System.Integer, _    Optional ByVal lArg As System.Integer, _    Optional ByVal bsNewName As System.String, _    Optional ByVal lEdmAddFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFileFromPath(     System.string bsSourcePath,    System.int lDestinationFolderID,    System.int lArg,    System.string bsNewName,    System.int lEdmAddFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFileFromPath(  &   System.String^ bsSourcePath, &   System.int lDestinationFolderID, &   System.int lArg, &   System.String^ bsNewName, &   System.int lEdmAddFlags ) ``` | |

#### Parameters

*bsSourcePath*
:   Path of file to add

*lDestinationFolderID*
:   ID of folder to which to add the file

*lArg*
:   Caller-defined argument

*bsNewName*
:   Optional new name of the added file

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