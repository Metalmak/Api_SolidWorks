<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~AddFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFile Method (IEdmBatchListing) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchListing Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html) : AddFile Method (IEdmBatchListing) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oIdOrPath*
:   ID or path of the file to add

*oFileDate*
:   Local file date

*lParam*
:   Caller-defined argument

*lEdmListFileFlags*
:   Reserved; must be 0

Adds a file to the batch of files for which to create a listing.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFile( _    ByVal oIdOrPath As System.Object, _    ByVal oFileDate As System.Date, _    ByVal lParam As System.Integer, _    Optional ByVal lEdmListFileFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFile(     System.object oIdOrPath,    System.DateTime oFileDate,    System.int lParam,    System.int lEdmListFileFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFile(  &   System.Object^ oIdOrPath, &   System.DateTime oFileDate, &   System.int lParam, &   System.int lEdmListFileFlags ) ``` | |

#### Parameters

*oIdOrPath*
:   ID or path of the file to add

*oFileDate*
:   Local file date

*lParam*
:   Caller-defined argument

*lEdmListFileFlags*
:   Reserved; must be 0

# ![](dotnetimages/collapse.gif)Remarks

After calling this method for each file whose properties you want to list, call [IEdmBatchListing::CreateList](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~CreateList.html) to create a listing for all the files.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchListing Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html)

[IEdmBatchListing Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional