<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData.html -->

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

| EdmUserData Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUserData Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [EdmUserData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2.html) in SOLIDWORKS PDM Professional 2010 and later.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmUserData     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmUserData : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmUserData : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmUserData{
  string [mbsUserName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mbsUserName.html);
  string [mbsInitials](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mbsInitials.html);
  string [mbsCompleteName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mbsCompleteName.html);
  string [mbsUserData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mbsUserData.html);
  string [mbsPassword](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mbsPassword.html);
  string [mbsEmail](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mbsEmail.html);
  integer [mlFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mlFlags.html);
  integer [mlSysRights](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mlSysRights.html);
  string [mbsColumnView](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mbsColumnView.html);
  integer [mlUserID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mlUserID.html);
  integer [mhStatus](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mhStatus.html);
  [IEdmUser6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser6.html)\* [mpoUser](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData~mpoUser.html);
};

# ![](dotnetimages/collapse.gif)Remarks

Holds information about a user. This struct is used as argument to [IEdmUserMgr6::AddUsers](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6~AddUsers.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmUserData Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007