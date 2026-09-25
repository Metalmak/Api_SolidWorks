<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCreateListExFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmCreateListExFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCreateListExFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options for creating lists used in calls to [IEdmBatchListing2::CreateListEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2~CreateListEx.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmCreateListExFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmCreateListExFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmCreateListExFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmclef\_AllConfigurations** | 2 = Return separate nodes for configurations |
| **Edmclef\_AsBuilt** | 16 = Use as-built reference versions instead of the latest version |
| **Edmclef\_DontGetLatest** | 64 = Do not get the latest version |
| **Edmclef\_GetDrawings** | 8 = Return drawings of added files |
| **Edmclef\_GetReferences** | 4 = Return references of added files |
| **Edmclef\_MayReadFiles** | 1 = Permit the API to read variables from the cached files; if this flag is not set, values are read from the database |
| **Edmclef\_Nothing** | 0 = Default behavior |
| **Edmclef\_ReturnReferences** | 32 = Return file references for every node that is passed in |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)