<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmBatchFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBatchFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags used in [IEdmBatchUpdate::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate~SetVar.html) and [IEdmBatchUpdate2::SetFolderVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~SetFolderVar.html) to control the behavior of [IEdmBatchUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate.html) and [IEdmBatchUpdate2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmBatchFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmBatchFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmBatchFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmBatch\_AllConfigs** | 1 = Ignore the configuration argument and update the variable value in all configurations |
| **EdmBatch\_Nothing** | 0 = Normal operation |
| **EdmBatch\_RefreshPreview** | 2 = Reload data card |
| **EdmBatch\_UpdateVarIfNotPartOfCard** | 4 = Update all variables, even those that are not visible in this data card |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)