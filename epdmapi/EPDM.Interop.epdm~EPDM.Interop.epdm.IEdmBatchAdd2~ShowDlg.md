<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd2~ShowDlg.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ShowDlg Method (IEdmBatchAdd2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchAdd2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd2.html) : ShowDlg Method (IEdmBatchAdd2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParentWnd*
:   Parent window handle for the dialog box

*lEdmAddFileDlgFlags*
:   Combination of [EdmAddFileDlgFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileDlgFlag.html) bits

*bsMessage*
:   Message to display in the dialog box

*bsCaption*
:   Dialog box caption

Shows a dialog box containing information about the file and folders that are about to be added to the vault by [IEdmBatchAdd::CommitAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~CommitAdd.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function ShowDlg( _    ByVal hParentWnd As System.Integer, _    ByVal lEdmAddFileDlgFlags As System.Integer, _    Optional ByVal bsMessage As System.String, _    Optional ByVal bsCaption As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ShowDlg(     System.int hParentWnd,    System.int lEdmAddFileDlgFlags,    System.string bsMessage,    System.string bsCaption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ShowDlg(  &   System.int hParentWnd, &   System.int lEdmAddFileDlgFlags, &   System.String^ bsMessage, &   System.String^ bsCaption ) ``` | |

#### Parameters

*hParentWnd*
:   Parent window handle for the dialog box

*lEdmAddFileDlgFlags*
:   Combination of [EdmAddFileDlgFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileDlgFlag.html) bits

*bsMessage*
:   Message to display in the dialog box

*bsCaption*
:   Dialog box caption

#### Return Value

True if the user clicked **OK**, false if the user clicked **Cancel**

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchAdd2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd2.html)

[IEdmBatchAdd2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009