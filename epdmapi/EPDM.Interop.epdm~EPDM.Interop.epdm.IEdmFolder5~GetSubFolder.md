<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetSubFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetSubFolder Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : GetSubFolder Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsFolderName*
:   Name of subfolder to get

Gets the interface to the subfolder with the specified name.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetSubFolder( _    ByVal bsFolderName As System.String _ ) As IEdmFolder5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmFolder5 GetSubFolder(     System.string bsFolderName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmFolder5^ GetSubFolder(  &   System.String^ bsFolderName ) ``` | |

#### Parameters

*bsFolderName*
:   Name of subfolder to get

#### Return Value

[IEdmFolder5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

# ![](dotnetimages/collapse.gif)Example

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

C++ users not using smart-pointer wrapper functions must release the returned pointer to IEdmFolder5.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FOLDER\_NOT\_FOUND: No subfolder with the specified name is found.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

[IEdmFolder5::ParentFolder Property ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~ParentFolder.html)

[IEdmFolder5::GetFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2