<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~CreateList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateList Method (IEdmBatchListing) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchListing Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html) : CreateList Method (IEdmBatchListing) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsColumnSetName*
:   Empty string, column set name returned by [IEdmBatchListing::GetColumnSetNames](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetColumnSetNames.html), or a list of variable names separated by a newline character and starting with a newline character (e.g., "\nAuthor\nProject\nDate")

*ppoColumns*
:   Array of [EdmListCol](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol.html) structures; one structure for each column in the column set; empty array if bsColumnSetName is an empty string

Obsolete. Superseded by [IEdmBatchListing2::CreateListEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2~CreateListEx.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CreateList( _    ByVal bsColumnSetName As System.String, _    ByRef ppoColumns() As EdmListCol _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void CreateList(     System.string bsColumnSetName,    out EdmListCol[] ppoColumns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CreateList(  &   System.String^ bsColumnSetName, &   [Out] array<EdmListCol>^ ppoColumns ) ``` | |

#### Parameters

*bsColumnSetName*
:   Empty string, column set name returned by [IEdmBatchListing::GetColumnSetNames](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetColumnSetNames.html), or a list of variable names separated by a newline character and starting with a newline character (e.g., "\nAuthor\nProject\nDate")

*ppoColumns*
:   Array of [EdmListCol](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol.html) structures; one structure for each column in the column set; empty array if bsColumnSetName is an empty string

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, call [IEdmBatchListing::GetFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetFiles.html) and [IEdmBatchListing::GetFolders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetFolders.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchListing Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html)

[IEdmBatchListing Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional