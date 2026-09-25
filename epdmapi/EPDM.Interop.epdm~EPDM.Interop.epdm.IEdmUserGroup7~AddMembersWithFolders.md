<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup7~AddMembersWithFolders.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddMembersWithFolders Method (IEdmUserGroup7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserGroup7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup7.html) : AddMembersWithFolders Method (IEdmUserGroup7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poMemberFolders*
:   Array of [EdmMemberFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMemberFolder.html) structures; one structure for each member folder to add to this user group

Adds the specified members of this user group to the specified folders.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddMembersWithFolders( _    ByVal poMemberFolders() As EdmMemberFolder _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddMembersWithFolders(     EdmMemberFolder[] poMemberFolders ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddMembersWithFolders(  &   array<EdmMemberFolder>^ poMemberFolders ) ``` | |

#### Parameters

*poMemberFolders*
:   Array of [EdmMemberFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMemberFolder.html) structures; one structure for each member folder to add to this user group

# ![](dotnetimages/collapse.gif)Example

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserGroup7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup7.html)

[IEdmUserGroup7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011