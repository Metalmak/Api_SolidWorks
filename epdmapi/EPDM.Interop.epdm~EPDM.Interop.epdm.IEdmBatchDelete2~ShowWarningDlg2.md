<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete2~ShowWarningDlg2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ShowWarningDlg2 Method (IEdmBatchDelete2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchDelete2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete2.html) : ShowWarningDlg2 Method (IEdmBatchDelete2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParentWnd*
:   Parent window handle for the dialog box

*bIncludeDeleted*
:   True to show the contents of the trash can, false to not

Shows a dialog box with the warnings and errors that occurred during [IEdmBatchDelete::ComputePermissions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~ComputePermissions.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function ShowWarningDlg2( _    ByVal hParentWnd As System.Integer, _    ByVal bIncludeDeleted As System.Boolean _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ShowWarningDlg2(     System.int hParentWnd,    System.bool bIncludeDeleted ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ShowWarningDlg2(  &   System.int hParentWnd, &   System.bool bIncludeDeleted ) ``` | |

#### Parameters

*hParentWnd*
:   Parent window handle for the dialog box

*bIncludeDeleted*
:   True to show the contents of the trash can, false to not

#### Return Value

True if the user chooses to continue the operation in spite of the warnings, false if the user cancels the operation

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmBatchDelete.ShowWarningDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~ShowWarningDlg.html) by adding the option to show the deleted objects in the trash can.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_NOT\_INITIALIZED: IEdmBatchDelete::ComputePermissions has not been called.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchDelete2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete2.html)

[IEdmBatchDelete2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009