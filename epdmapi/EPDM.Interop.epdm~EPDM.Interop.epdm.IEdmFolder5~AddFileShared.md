<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFileShared.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFileShared Method (IEdmFolder5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : AddFileShared Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of file to share

*lParentWindow*
:   Parent window handle

Shares a file in another folder with this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFileShared( _    ByVal lFileID As System.Integer, _    ByVal lParentWindow As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFileShared(     System.int lFileID,    System.int lParentWindow ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFileShared(  &   System.int lFileID, &   System.int lParentWindow ) ``` | |

#### Parameters

*lFileID*
:   ID of file to share

*lParentWindow*
:   Parent window handle

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_NAME\_ALREADY\_EXISTS: There is already a file with the same name in this folder.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: One of the installed [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html).EdmCmd\_PreShare hooks did not permit the operation.* E\_EDM\_FILE\_NOT\_FOUND: The source file was not found. (The ID is invalid.)* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to share the specified file.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

[IEdmFolder5::AddFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFile.html)

[IEdmFolder5::CopyFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CopyFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2