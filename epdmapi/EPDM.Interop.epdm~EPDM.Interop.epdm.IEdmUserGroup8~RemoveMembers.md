<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup8~RemoveMembers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RemoveMembers Method (IEdmUserGroup8) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserGroup8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup8.html) : RemoveMembers Method (IEdmUserGroup8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poMemberFolders*
:   Array of [EdmMemberFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMemberFolder.html) structures; one structure for each member to remove from this user group

Removes the specified members from this user group.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub RemoveMembers( _    ByVal poMemberFolders() As EdmMemberFolder _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void RemoveMembers(     EdmMemberFolder[] poMemberFolders ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RemoveMembers(  &   array<EdmMemberFolder>^ poMemberFolders ) ``` | |

#### Parameters

*poMemberFolders*
:   Array of [EdmMemberFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMemberFolder.html) structures; one structure for each member to remove from this user group

# ![](dotnetimages/collapse.gif)Example

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserGroup8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup8.html)

[IEdmUserGroup8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2012