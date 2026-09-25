<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6~AddMembers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddMembers Method (IEdmUserGroup6) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserGroup6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6.html) : AddMembers Method (IEdmUserGroup6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poUserIDs*
:   Array of database IDs of users to add to this user group (see **Remarks**)

Adds the specified users to this user group.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddMembers( _    ByVal poUserIDs() As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddMembers(     System.int[] poUserIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddMembers(  &   System.array<int>^ poUserIDs ) ``` | |

#### Parameters

*poUserIDs*
:   Array of database IDs of users to add to this user group (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call IEdmUser5::[ID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5~ID.html) to populate the array of poUserIDs.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserGroup6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6.html)

[IEdmUserGroup6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010