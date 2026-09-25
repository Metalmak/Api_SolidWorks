<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponentFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmRevComponentFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRevComponentFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags used to control the members of the struct [EdmRevComponent2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmRevComponentFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmRevComponentFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmRevComponentFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmrcf\_EndOfListContinue** | 4 = Continue to use the last list item when the end of the list is reached |
| **Edmrcf\_EndOfListRestart** | 2 = Restart from the first list item when the end of the list is reached |
| **Edmrcf\_EndOfListSendMail** | 16 = Send mail to a user or group when the end of the list is reached; the recipient ID is stored in the EdmRevcomponent2 [mlRecipientID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mlRecipientID.html) struct field |
| **Edmrcf\_EndOfListStop** | 8 = Halt the operation when the end of the list is reached |
| **Edmrcf\_RecipientIsGroup** | 1 = EdmRevcomponent2 [mlRecipientID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mlRecipientID.html) struct field is a group ID; this flag is only used in combination with Edmrcf\_EndOflistSendMail |
| **Edmrcf\_TypeFormatString** | 32 = Revision number is of type *format string* |
| **Edmrcf\_TypeList** | 64 = Revision number is of type *list* |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)