<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2~CreateListEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateListEx Method (IEdmBatchListing2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchListing2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2.html) : CreateListEx Method (IEdmBatchListing2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsColumnSetName*
:   Empty string, one of the set names returned by [IEdmBatchListing::GetColumnSetNames](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetColumnSetNames.html), or a list of variable names separated by newline characters and starting with a newline character (e.g., "\nAuthor\nProject\nDate")

*lEdmCreateListExFlags*
:   Combination of [EdmCreateListExFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCreateListExFlags.html) bits

*ppoColumns*
:   Array of [EdmListCol](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol.html) structures; one structure for each column in the column set

*poAux*
:   Reserved for future use

Creates a listing of the properties of the files and folders that were added to the batch using [IEdmBatchListing::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~AddFile.html), [IEdmBatchListing::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~AddFolder.html), and [IEdmBatchListing2::AddFileCfg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2~AddFileCfg.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CreateListEx( _    ByVal bsColumnSetName As System.String, _    ByVal lEdmCreateListExFlags As System.Integer, _    ByRef ppoColumns() As EdmListCol, _    Optional ByVal poAux As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void CreateListEx(     System.string bsColumnSetName,    System.int lEdmCreateListExFlags,    out EdmListCol[] ppoColumns,    System.object poAux ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CreateListEx(  &   System.String^ bsColumnSetName, &   System.int lEdmCreateListExFlags, &   [Out] array<EdmListCol>^ ppoColumns, &   System.Object^ poAux ) ``` | |

#### Parameters

*bsColumnSetName*
:   Empty string, one of the set names returned by [IEdmBatchListing::GetColumnSetNames](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~GetColumnSetNames.html), or a list of variable names separated by newline characters and starting with a newline character (e.g., "\nAuthor\nProject\nDate")

*lEdmCreateListExFlags*
:   Combination of [EdmCreateListExFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCreateListExFlags.html) bits

*ppoColumns*
:   Array of [EdmListCol](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol.html) structures; one structure for each column in the column set

*poAux*
:   Reserved for future use

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method extends [IEdmBatchListing::CreateList](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~CreateList.html) by adding the ability to configure from where the file variables are read.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchListing2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2.html)

[IEdmBatchListing2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009