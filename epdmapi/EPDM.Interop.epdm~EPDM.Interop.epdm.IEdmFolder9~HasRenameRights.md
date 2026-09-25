<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder9~HasRenameRights.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| HasRenameRights Method (IEdmFolder9) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder9.html) : HasRenameRights Method (IEdmFolder9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*lFileID*
:   ID of the file to rename

*bsOldFileName*
:   Old file name

*bsRenamedFileName*
:   New file name

*pbSilent*
:   True to silently check for permissions to rename the file (i.e., do not display message box), false to not

Gets whether the user has permission to rename the specified file in this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function HasRenameRights( _    ByVal lParentWnd As System.Integer, _    ByVal lFileID As System.Integer, _    ByVal bsOldFileName As System.String, _    ByVal bsRenamedFileName As System.String, _    ByVal pbSilent As System.Boolean _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool HasRenameRights(     System.int lParentWnd,    System.int lFileID,    System.string bsOldFileName,    System.string bsRenamedFileName,    System.bool pbSilent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool HasRenameRights(  &   System.int lParentWnd, &   System.int lFileID, &   System.String^ bsOldFileName, &   System.String^ bsRenamedFileName, &   System.bool pbSilent ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*lFileID*
:   ID of the file to rename

*bsOldFileName*
:   Old file name

*bsRenamedFileName*
:   New file name

*pbSilent*
:   True to silently check for permissions to rename the file (i.e., do not display message box), false to not

#### Return Value

True if the user has permission to rename the specified file, false if not

# ![](dotnetimages/collapse.gif)Example

[Add Files to Vault (VB.NET)](Add_Files_to_Vault_Example_VBNET.htm)

[Add Files to Vault (C#)](Add_Files_to_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder9.html)

[IEdmFolder9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2016