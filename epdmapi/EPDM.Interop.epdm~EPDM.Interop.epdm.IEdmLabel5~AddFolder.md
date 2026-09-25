<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5~AddFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFolder Method (IEdmLabel5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmLabel5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5.html) : AddFolder Method (IEdmLabel5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFolderID*
:   ID of folder on which to set this label

*bRecursive*
:   True to recursively set this label on all subfolders, false to not

Sets this label on the specified folder and all of the files in that folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFolder( _    ByVal lFolderID As System.Integer, _    ByVal bRecursive As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFolder(     System.int lFolderID,    System.bool bRecursive ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFolder(  &   System.int lFolderID, &   System.bool bRecursive ) ``` | |

#### Parameters

*lFolderID*
:   ID of folder on which to set this label

*bRecursive*
:   True to recursively set this label on all subfolders, false to not

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmLabel5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5.html)

[IEdmLabel5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2