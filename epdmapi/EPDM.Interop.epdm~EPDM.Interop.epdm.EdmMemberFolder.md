<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMemberFolder.html -->

![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/drpdown.gif)
![](dotnetimages/drpdown_orange.gif)
![](dotnetimages/copycode.gif)
![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |

| EdmMemberFolder Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMemberFolder_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmMemberFolder Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Adds a user as a member of a group to a specific folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmMemberFolder     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmMemberFolder : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmMemberFolder : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmMemberFolder{
  integer [mlUserID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMemberFolder~mlUserID.html);
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMemberFolder~mlFolderID.html);
};

# ![](dotnetimages/collapse.gif)Example

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Used by [IEdmUserGroup7::AddMembersWithFolders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup7~AddMembersWithFolders.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmMemberFolder Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMemberFolder_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011