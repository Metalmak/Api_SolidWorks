<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~Rename.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rename Method (IEdmFile5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : Rename Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*bsName*
:   New file name

*bRenameLocalCopies*
:   Optional; true to rename local copies, false to not; default is true

Obsolete. Superseded by [IEdmFile6::RenameEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6~RenameEx.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rename( _    ByVal lParentWnd As System.Integer, _    ByVal bsName As System.String, _    Optional ByVal bRenameLocalCopies As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rename(     System.int lParentWnd,    System.string bsName,    System.bool bRenameLocalCopies ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rename(  &   System.int lParentWnd, &   System.String^ bsName, &   System.bool bRenameLocalCopies ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*bsName*
:   New file name

*bRenameLocalCopies*
:   Optional; true to rename local copies, false to not; default is true

# ![](dotnetimages/collapse.gif)Remarks

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* E\_EDM\_NAME\_ALREADY\_EXISTS: The specified name already exists.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to rename this file.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2