<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmUserDataFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUserDataFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags used in [EdmUserData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData.html)'s mlFlags field when adding users with [IEdmUserMgr6::AddUsers](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6~AddUsers.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmUserDataFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmUserDataFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmUserDataFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmudf\_CopySettings** | 4 = Copy the settings from the user with EdmUserData.mlUserID |
| **Edmudf\_ForceAdd** | 2 = Add this user even if other users in the array sent to [IEdmUserMgr7::AddUsers2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~AddGroups2.html) cannot be added |
| **Edmudf\_GetInterface** | 1 = Return the [IEdmUser6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser6.html) interface in the structure |
| **Edmudf\_Nothing** | 0 = None of the other flags |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)