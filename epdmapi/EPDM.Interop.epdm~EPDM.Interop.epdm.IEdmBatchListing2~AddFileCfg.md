<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2~AddFileCfg.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFileCfg Method (IEdmBatchListing2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchListing2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2.html) : AddFileCfg Method (IEdmBatchListing2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oIdOrPath*
:   Path of file to add

*oFileDate*
:   Local file date

*lParam*
:   Caller-defined argument

*bsConfigName*
:   Name of the configuration from which to read the file variables; default is an empty string

*lEdmListFileFlags*
:   Combination of [EdmListFileFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFileFlags.html) bits; default is 0

Adds a file to the batch of files for which to create a listing using variables from the specified configuration.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFileCfg( _    ByVal oIdOrPath As System.Object, _    ByVal oFileDate As System.Date, _    ByVal lParam As System.Integer, _    Optional ByVal bsConfigName As System.String, _    Optional ByVal lEdmListFileFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFileCfg(     System.object oIdOrPath,    System.DateTime oFileDate,    System.int lParam,    System.string bsConfigName,    System.int lEdmListFileFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFileCfg(  &   System.Object^ oIdOrPath, &   System.DateTime oFileDate, &   System.int lParam, &   System.String^ bsConfigName, &   System.int lEdmListFileFlags ) ``` | |

#### Parameters

*oIdOrPath*
:   Path of file to add

*oFileDate*
:   Local file date

*lParam*
:   Caller-defined argument

*bsConfigName*
:   Name of the configuration from which to read the file variables; default is an empty string

*lEdmListFileFlags*
:   Combination of [EdmListFileFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFileFlags.html) bits; default is 0

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method extends IEdmBatchListing::AddFile and IEdmBAtchListing::AddFolder by adding the ability to specify the configuration from which to read the file variables.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchListing2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2.html)

[IEdmBatchListing2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009