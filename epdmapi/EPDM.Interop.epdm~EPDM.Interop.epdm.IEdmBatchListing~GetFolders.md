<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetFolders.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFolders Method (IEdmBatchListing) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchListing Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html) : GetFolders Method (IEdmBatchListing) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoFolders*
:   Array of [EdmListFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolder.html) structures; one structure for each folder in the listing

Gets all the folders in this listing.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetFolders( _    ByRef ppoFolders() As EdmListFolder _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFolders(     out EdmListFolder[] ppoFolders ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFolders(  &   [Out] array<EdmListFolder>^ ppoFolders ) ``` | |

#### Parameters

*ppoFolders*
:   Array of [EdmListFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolder.html) structures; one structure for each folder in the listing

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IEdmBatchListing::CreateList](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~CreateList.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchListing Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html)

[IEdmBatchListing Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010