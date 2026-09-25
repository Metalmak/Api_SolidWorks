<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2.html -->

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

| EdmUserData2 Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUserData2 Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a user to be created.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmUserData2     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmUserData2 : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmUserData2 : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmUserData2{
  string   [mbsUserName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mbsUserName.html);
  string   [mbsInitials](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mbsInitials.html);
  string   [mbsCompleteName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mbsCompleteName.html);
  string   [mbsUserData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mbsUserData.html);
  string   [mbsPassword](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mbsPassword.html);
  string   [mbsEmail](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mbsEmail.html);
  integer   [mlFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mlFlags.html);
  [EdmSysPerm](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html)[] [moSysPerms](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~moSysPerms.html);
  string   [mbsColumnView](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mbsColumnView.html);
  integer   [mlUserID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mlUserID.html);
  integer   [mhStatus](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mhStatus.html);
  [IEdmUser6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser6.html)\* [mpoUser](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2~mpoUser.html);
};

# ![](dotnetimages/collapse.gif)Example

[Add Users (C#)](Add_Users_Example_CSharp.htm)

[Add Users (VB.NET)](Add_Users_Example_VBNET.htm)

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmUserData2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010