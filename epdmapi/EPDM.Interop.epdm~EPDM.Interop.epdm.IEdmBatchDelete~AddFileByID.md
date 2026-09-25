<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFileByID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFileByID Method (IEdmBatchDelete) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchDelete Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html) : AddFileByID Method (IEdmBatchDelete) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of file to delete

*lFolderID*
:   ID of file's parent folder

Adds a file with the specified file and folder IDs to the batch of files to be deleted.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFileByID( _    ByVal lFileID As System.Integer, _    ByVal lFolderID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFileByID(     System.int lFileID,    System.int lFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFileByID(  &   System.int lFileID, &   System.int lFolderID ) ``` | |

#### Parameters

*lFileID*
:   ID of file to delete

*lFolderID*
:   ID of file's parent folder

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, call [IEdmBatchDelete::CommitDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~CommitDelete.html) to delete the file from the vault.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchDelete Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html)

[IEdmBatchDelete Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008