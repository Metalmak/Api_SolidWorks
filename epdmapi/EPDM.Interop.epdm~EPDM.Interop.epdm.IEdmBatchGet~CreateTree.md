<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~CreateTree.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateTree Method (IEdmBatchGet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchGet Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html) : CreateTree Method (IEdmBatchGet) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*lEdmGetCmdFlags*
:   Combination of [EdmGetCmdFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetCmdFlags.html) bits; specifies options for retrieving files from the vault

Computes the file reference tree with the files added to the batch using [IEdmBatchGet::AddSelection](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~AddSelection.html) or [IEdmBatchGet::AddSelectionEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~AddSelectionEx.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CreateTree( _    ByVal lParentWnd As System.Integer, _    ByVal lEdmGetCmdFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void CreateTree(     System.int lParentWnd,    System.int lEdmGetCmdFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CreateTree(  &   System.int lParentWnd, &   System.int lEdmGetCmdFlags ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*lEdmGetCmdFlags*
:   Combination of [EdmGetCmdFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetCmdFlags.html) bits; specifies options for retrieving files from the vault

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchGet](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, call [IEdmBatchGet::ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~ShowDlg.html) and [IEdmBatchGet::GetFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~GetFiles.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchGet Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html)

[IEdmBatchGet Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional