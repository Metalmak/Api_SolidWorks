<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6~AddFiles.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFiles Method (IEdmFolder6) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6.html) : AddFiles Method (IEdmFolder6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*ppoFiles*
:   Array of [EdmAddFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo.html) structures; one structure for each added file

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) to control this add operation and obtain progress information about it

Adds one or more files to this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFiles( _    ByVal lParentWnd As System.Integer, _    ByRef ppoFiles() As EdmAddFileInfo, _    ByVal poCallback As IEdmCallback6 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFiles(     System.int lParentWnd,    out EdmAddFileInfo[] ppoFiles,    IEdmCallback6 poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFiles(  &   System.int lParentWnd, &   [Out] array<EdmAddFileInfo>^ ppoFiles, &   IEdmCallback6^ poCallback ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*ppoFiles*
:   Array of [EdmAddFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo.html) structures; one structure for each added file

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) to control this add operation and obtain progress information about it

# ![](dotnetimages/collapse.gif)Example

[Add Files to Vault (VB.NET)](Add_Files_to_Vault_Example_VBNET.htm)

[Add Files to Vault (C#)](Add_Files_to_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is more efficient than [IEdmFolder5::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFile.html) when adding many files.

Before calling this method, call [IFolder12::SetFileNameSerNo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder12~SetFileNameSerNo.html) for each new file to specify how to create the name of the new file's data card.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_SN\_FILE: The operation needs to generate serial numbers from a file but the end of the file has been reached.* E\_EDM\_SN\_FILE\_NOT\_FOUND: The operation needs to generate serial numbers from a file that cannot be found.* E\_EDM\_CANCELLED\_BY\_USER: The operation was cancelled via the optional callback interface.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6.html)

[IEdmFolder6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0