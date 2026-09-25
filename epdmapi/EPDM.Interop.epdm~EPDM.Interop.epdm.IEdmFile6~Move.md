<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6~Move.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Move Method (IEdmFile6) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6.html) : Move Method (IEdmFile6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*lParentID*
:   ID of the source folder

*lNewParentID*
:   ID of the destination folder

*lFlags*
:   0; reserved

Moves this file to another location in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Move( _    ByVal lParentWnd As System.Integer, _    ByVal lParentID As System.Integer, _    ByVal lNewParentID As System.Integer, _    ByVal lFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Move(     System.int lParentWnd,    System.int lParentID,    System.int lNewParentID,    System.int lFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Move(  &   System.int lParentWnd, &   System.int lParentID, &   System.int lNewParentID, &   System.int lFlags ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*lParentID*
:   ID of the source folder

*lNewParentID*
:   ID of the destination folder

*lFlags*
:   0; reserved

# ![](dotnetimages/collapse.gif)Example

[Add Files to Vault (VB.NET)](Add_Files_to_Vault_Example_VBNET.htm)

[Add Files to Vault (C#)](Add_Files_to_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the file has references, the paths of those references are updated to match the new location. If the file is being referenced by other files, the referencing files are updated to point to the new location.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.* E\_EDM\_MOVE\_FILE\_PERMISSION\_DENIED: The user does not have permission to move the file.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6.html)

[IEdmFile6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0