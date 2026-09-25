<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateFileListFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmChangeStateFileListFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmChangeStateFileListFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options for returning files when making calls to [IEdmBatchChangeState::GetFileList](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~GetFileList.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmChangeStateFileListFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmChangeStateFileListFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmChangeStateFileListFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Ecsflf\_GetActionUpdated** | 4 = Return files that were updated by an action that set a variable value |
| **Ecsflf\_GetChanged** | 1 = Return files that had their state changed |
| **Ecsflf\_GetUnprocessed** | 2 = Return files that did not have their state changed |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)