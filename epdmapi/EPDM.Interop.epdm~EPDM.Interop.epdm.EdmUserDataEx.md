<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx.html -->

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

| EdmUserDataEx Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUserDataEx Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a user.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmUserDataEx     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmUserDataEx : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmUserDataEx : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmUserDataEx{
  integer [mlUserID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mlUserID.html);
  integer [mlEdmUserDataExFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mlEdmUserDataExFlags.html);
  string [mbsInitials](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsInitials.html);
  string [mbsCompleteName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsCompleteName.html);
  string [mbsUserData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsUserData.html);
  string [mbsEmail](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsEmail.html);
  string [mbsPhone](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsPhone.html);
  string [mbsCellPhone](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsCellPhone.html);
  string [mbsPicturePath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsPicturePath.html);
  string [mbsWebSite1](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsWebSite1.html);
  string [mbsWebSite2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsWebSite2.html);
  string [mbsWebSite3](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsWebSite3.html);
  string [mbsWebSite4](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsWebSite4.html);
  string [mbsPresenceNote](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsPresenceNote.html);
};

# ![](dotnetimages/collapse.gif)Example

[Find Users (VB.NET)](Find_Users_Example_VBNET.htm)

[Find Users (C#)](Find_Users_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Used to read/write user properties via [IEdmUser10::GetUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~GetUserDataEx.html) and [IEdmUser10::SetUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~SetUserDataEx.html).

The following image shows where the EdmUserDataEx struct fields are used in the user popup window when [IEdmUserMgr8::ShowUserPopup](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8~ShowUserPopup.html) is called after updating the properties with [IEdmUser10::GetUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~GetUserDataEx.html).

![](UserPopup.png)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmUserDataEx Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013