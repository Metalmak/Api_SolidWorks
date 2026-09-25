<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataExFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmUserDataExFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUserDataExFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags that tell which members of [EdmUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx.html) are valid. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmUserDataExFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmUserDataExFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmUserDataExFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmudex\_All** | A combination of all the other flags  **NOTE**: To get better performance, call [IEdmUser10::GetUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~GetUserDataEx.html) and only specify the enumerators that you need. |
| **Edmudex\_CellPhone** | 32 = mbsCellPhone of EdmUserDataEx is valid |
| **Edmudex\_CompleteName** | 2 = mbsCompleteName of EdmUserDataEx is valid |
| **Edmudex\_Email** | 8 = mbsEmail of EdmUserDataEx is valid |
| **Edmudex\_Initials** | 1 = mbsInitials of EdmUserDataEx is valid |
| **Edmudex\_Nothing** | 0 = None of EdmUserDataEx members are valid |
| **Edmudex\_Phone** | 16 = mbsPhone of EdmUserDataEx is valid |
| **Edmudex\_PicturePath** | 64 = mbsPicturePath of EdmUserDataEx is valid |
| **Edmudex\_PresenceNote** | 2048 = mbsPresenceNote of EdmUserDataEx is valid |
| **Edmudex\_UserData** | 4 = mbsUserData of EdmUserDataEx is valid |
| **Edmudex\_WebSite1** | 128 = mbsWebSite1 of EdmUserDataEx is valid |
| **Edmudex\_WebSite2** | 256 = mbsWebSite2 of EdmUserDataEx is valid |
| **Edmudex\_WebSite3** | 512 = mbsWebSite3 of EdmUserDataEx is valid |
| **Edmudex\_WebSite4** | 1024 = mbsWebSite4 of EdmUserDataEx is valid |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmUser10::SetUserDataEx Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~SetUserDataEx.html)