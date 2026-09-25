<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMBoxType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmMBoxType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmMBoxType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of widget to insert or display in [IEdmVault5::MsgBox](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~MsgBox.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmMBoxType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmMBoxType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmMBoxType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmMbt\_AbortRetryIgnore** | 2 = Insert **Abort**, **Retry,** and **Ignore** |
| **EdmMbt\_Icon\_Information** | 64 = Display the information icon |
| **EdmMbt\_Icon\_Question** | 32 = Display the question icon |
| **EdmMbt\_Icon\_Warning** | 48 = Display the warning icon |
| **EdmMbt\_OKCancel** | 1 = Insert **OK** and **Cancel** |
| **EdmMbt\_OKOnly** | 0 = Insert **OK** |
| **EdmMbt\_RetryCancel** | 5 = Insert **Retry** and **Cancel** |
| **EdmMbt\_YesNo** | 4 = Insert **Yes** and **No** |
| **EdmMbt\_YesNoCancel** | 3 = Insert **Yes**, **No**, and **Cancel** |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)