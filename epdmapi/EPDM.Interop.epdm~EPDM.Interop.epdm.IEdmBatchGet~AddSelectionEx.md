<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~AddSelectionEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddSelectionEx Method (IEdmBatchGet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchGet Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html) : AddSelectionEx Method (IEdmBatchGet) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); vault from which to get the file

*lFileID*
:   ID of file to get

*lParentFolderID*
:   ID of the file's parent folder

*oVersionOrFileDate*
:   Number or modified date of the version of the file to get

Adds a file with the specified ID and version to the batch of files to get.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddSelectionEx( _    ByVal poVault As EdmVault5, _    ByVal lFileID As System.Integer, _    ByVal lParentFolderID As System.Integer, _    ByVal oVersionOrFileDate As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddSelectionEx(     EdmVault5 poVault,    System.int lFileID,    System.int lParentFolderID,    System.object oVersionOrFileDate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddSelectionEx(  &   EdmVault5^ poVault, &   System.int lFileID, &   System.int lParentFolderID, &   System.Object^ oVersionOrFileDate ) ``` | |

#### Parameters

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); vault from which to get the file

*lFileID*
:   ID of file to get

*lParentFolderID*
:   ID of the file's parent folder

*oVersionOrFileDate*
:   Number or modified date of the version of the file to get

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchGet Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html)

[IEdmBatchGet Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional