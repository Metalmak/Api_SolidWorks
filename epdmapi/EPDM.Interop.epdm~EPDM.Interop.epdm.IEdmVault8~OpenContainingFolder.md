<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8~OpenContainingFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| OpenContainingFolder Method (IEdmVault8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8.html) : OpenContainingFolder Method (IEdmVault8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oFilePathOrID*
:   ID or path of file to select; 0 to ignore (see **Remarks**)

*oFolderPathOrID*
:   ID or path of folder on which to open File Explorer; 0 to ignore

Opens File Explorer on the specified folder and selects the specified file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub OpenContainingFolder( _    ByVal oFilePathOrID As System.Object, _    Optional ByVal oFolderPathOrID As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void OpenContainingFolder(     System.object oFilePathOrID,    System.object oFolderPathOrID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OpenContainingFolder(  &   System.Object^ oFilePathOrID, &   System.Object^ oFolderPathOrID ) ``` | |

#### Parameters

*oFilePathOrID*
:   ID or path of file to select; 0 to ignore (see **Remarks**)

*oFolderPathOrID*
:   ID or path of folder on which to open File Explorer; 0 to ignore

# ![](dotnetimages/collapse.gif)Example

|  |  |
| --- | --- |
| OpenContainingFolder 102, 33 | Opens folder with ID, 33, and selects file with ID, 102. |
| OpenContainingFolder “c:\TheVault\SubFolder\test.txt” | Opens folder, SubFolder, and selects file, test.txt. |
| OpenContainingFolder 0, 45 | Opens the parent folder of folder with ID, 45, and selects the folder with ID, 45. |
| OpenContainingFolder 321, 0 | Opens first folder where file with ID, 321, is found and selects the file. |
| OpenContainingFolder 0, “c:\TheVault\SubFolder” | Opens the vault root folder and selects the folder, SubFolder. |

# ![](dotnetimages/collapse.gif)Remarks

If oFilePathOrID is a path to a file, oFolderPathOrID is ignored.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8.html)

[IEdmVault8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4