<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault19~CopyTree.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CopyTree Method (IEdmVault19) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault19 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault19.html) : CopyTree Method (IEdmVault19) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lSrcFileID*
:   ID of the assembly to copy

*lSrcFileProjID*
:   ID of the parent folder of lSrcFileID; only valid if lSrcFileID is not 0 or blank

*lDestinationFolderPath*
:   Full path name of destination folder

*vbShowDlg*
:   True to display the copy dialog, false to not

*vbShowProgressBar*
:   True to display a progress bar during the copy procedure, false to not

*oCopyTreeOptions*
:   Copy tree options as defined in [EdmCopyTreeOptions](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyTreeOptions.html)

*lHwnd*
:   Parent window handle

Copies the specified assembly and its referenced parts and drawings to the specified destination folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CopyTree( _    ByVal lSrcFileID As System.Integer, _    ByVal lSrcFileProjID As System.Integer, _    ByVal lDestinationFolderPath As System.String, _    ByVal vbShowDlg As System.Boolean, _    ByVal vbShowProgressBar As System.Boolean, _    ByVal oCopyTreeOptions As EdmCopyTreeOptions, _    ByVal lHwnd As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void CopyTree(     System.int lSrcFileID,    System.int lSrcFileProjID,    System.string lDestinationFolderPath,    System.bool vbShowDlg,    System.bool vbShowProgressBar,    EdmCopyTreeOptions oCopyTreeOptions,    System.int lHwnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CopyTree(  &   System.int lSrcFileID, &   System.int lSrcFileProjID, &   System.String^ lDestinationFolderPath, &   System.bool vbShowDlg, &   System.bool vbShowProgressBar, &   EdmCopyTreeOptions oCopyTreeOptions, &   System.int lHwnd ) ``` | |

#### Parameters

*lSrcFileID*
:   ID of the assembly to copy

*lSrcFileProjID*
:   ID of the parent folder of lSrcFileID; only valid if lSrcFileID is not 0 or blank

*lDestinationFolderPath*
:   Full path name of destination folder

*vbShowDlg*
:   True to display the copy dialog, false to not

*vbShowProgressBar*
:   True to display a progress bar during the copy procedure, false to not

*oCopyTreeOptions*
:   Copy tree options as defined in [EdmCopyTreeOptions](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyTreeOptions.html)

*lHwnd*
:   Parent window handle

# ![](dotnetimages/collapse.gif)Example

See the [IEdmVault19](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault19.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault19 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault19.html)

[IEdmVault19 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault19_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018