<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~GetFiles.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFiles Method (IEdmBatchGet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchGet Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html) : GetFiles Method (IEdmBatchGet) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*poCallback*
:   Optional pointer to a class that implements [IEdmGetOpCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html), [IEdmGetOpCallback2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback2.html), or [IEdmGetOpCallback3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback3.html) to control and monitor the operation

Gets the files in the batch.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetFiles( _    ByVal lParentWnd As System.Integer, _    Optional ByVal poCallback As IEdmGetOpCallback _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFiles(     System.int lParentWnd,    IEdmGetOpCallback poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFiles(  &   System.int lParentWnd, &   IEdmGetOpCallback^ poCallback ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*poCallback*
:   Optional pointer to a class that implements [IEdmGetOpCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html), [IEdmGetOpCallback2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback2.html), or [IEdmGetOpCallback3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback3.html) to control and monitor the operation

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchGet](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call this method after calling [IEdmBatchGet::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~CreateTree.html) and, optionally, [IEdmBatchGet::ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~ShowDlg.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchGet Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html)

[IEdmBatchGet Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional