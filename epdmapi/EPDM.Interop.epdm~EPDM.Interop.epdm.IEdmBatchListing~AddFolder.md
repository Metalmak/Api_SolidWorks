<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~AddFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFolder Method (IEdmBatchListing) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchListing Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html) : AddFolder Method (IEdmBatchListing) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oIdOrPath*
:   ID of folder to add; path is not supported in SOLIDWORKS PDM 2010

*lParam*
:   Caller-defined argument

*lEdmListFolderFlags*
:   Only [EdmListFiolderFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolderFlags.html).EdmListFolder\_Recursive is supported

Adds a folder to the batch of folders for which to create a listing.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFolder( _    ByVal oIdOrPath As System.Object, _    ByVal lParam As System.Integer, _    Optional ByVal lEdmListFolderFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFolder(     System.object oIdOrPath,    System.int lParam,    System.int lEdmListFolderFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFolder(  &   System.Object^ oIdOrPath, &   System.int lParam, &   System.int lEdmListFolderFlags ) ``` | |

#### Parameters

*oIdOrPath*
:   ID of folder to add; path is not supported in SOLIDWORKS PDM 2010

*lParam*
:   Caller-defined argument

*lEdmListFolderFlags*
:   Only [EdmListFiolderFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolderFlags.html).EdmListFolder\_Recursive is supported

# ![](dotnetimages/collapse.gif)Remarks

After calling this method for each folder whose properties you want to list, call [IEdmBatchListing::CreateList](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~CreateList.html) to create a listing of all the folders' properties.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchListing Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html)

[IEdmBatchListing Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM 2010