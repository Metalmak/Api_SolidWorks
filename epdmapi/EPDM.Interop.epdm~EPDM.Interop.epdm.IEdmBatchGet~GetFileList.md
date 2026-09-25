<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~GetFileList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFileList Method (IEdmBatchGet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchGet Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html) : GetFileList Method (IEdmBatchGet) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lEdmGetFileListFlags*
:   Combination of [EdmGetFileListFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFileListFlag.html) bits

Gets a list of the files in this batch.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFileList( _    ByVal lEdmGetFileListFlags As System.Integer _ ) As EdmSelectionList5 ``` | |

| C# |  |
| --- | --- |
| ``` EdmSelectionList5 GetFileList(     System.int lEdmGetFileListFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmSelectionList5^ GetFileList(  &   System.int lEdmGetFileListFlags ) ``` | |

#### Parameters

*lEdmGetFileListFlags*
:   Combination of [EdmGetFileListFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFileListFlag.html) bits

#### Return Value

[IEdmSelectionList5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html); list of files in this batch

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchGet](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchGet Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html)

[IEdmBatchGet Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional