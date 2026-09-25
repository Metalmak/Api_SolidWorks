<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockOpReply.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmUnlockOpReply Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUnlockOpReply Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of operations returned from your [IEdmUnlockOpCallback::MsgBox](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~MsgBox.html) method if you implement an [IEdmUnlockOpCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html) interface to use with the [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) interface.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmUnlockOpReply     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmUnlockOpReply : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmUnlockOpReply : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Euor\_Cancel** | 1 = Cancel the entire operation |
| **Euor\_ClearVar** | 10 = Clear the value of the conflicting unique variable |
| **Euor\_Error** | -1 = Internal error code; typically not returned by you |
| **Euor\_OK** | 0 = Continue the operation |
| **Euor\_Retry** | 12 = Retry operation |
| **Euor\_SkipFile** | 11 = Continue the operation, but skip this particular file |

# ![](dotnetimages/collapse.gif)Remarks

The return value tells SOLIDWORKS PDM Professional what to do.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)