<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMsgType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmMsgType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmMsgType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of messages sent to a user.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmMsgType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmMsgType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmMsgType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmMsgType\_ExternalNotification** | 4 = The message is an external notification |
| **EdmMsgType\_FileNotification** | 2 = The message is a file notification |
| **EdmMsgType\_FolderNotification** | 3 = The message is a folder notification |
| **EdmMsgType\_Invalid** | 0 = Invalid message (internal error code) |
| **EdmMsgType\_UserMessage** | 1 = The message is a file notification |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmMessage5::MessageType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMessage5~MessageType.html)