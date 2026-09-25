<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing4~GetFiles2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFiles2 Method (IEdmBatchListing4) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchListing4 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing4.html) : GetFiles2 Method (IEdmBatchListing4) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoFiles*
:   Array of [EdmListFile2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2.html) structures; one structure for each file in the listing

Gets all the files in this listing.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetFiles2( _    ByRef ppoFiles() As EdmListFile2 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFiles2(     out EdmListFile2[] ppoFiles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFiles2(  &   [Out] array<EdmListFile2>^ ppoFiles ) ``` | |

#### Parameters

*ppoFiles*
:   Array of [EdmListFile2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2.html) structures; one structure for each file in the listing

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method does not work with assemblies that contain weldment components or cutlist items.

Before calling this method, call [IEdmBatchListing2::CreateListEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2~CreateListEx.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchListing4 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing4.html)

[IEdmBatchListing4 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing4_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017