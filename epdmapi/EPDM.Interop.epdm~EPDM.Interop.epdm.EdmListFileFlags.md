<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFileFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmListFileFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmListFileFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags passed to [IEdmBatchListing::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~AddFile.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmListFileFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmListFileFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmListFileFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmList\_IsCutListItem** | 2 = The file is a cut list item in another file |
| **EdmList\_IsInternalComponent** | 4 = The file is a virtual component in another file |
| **EdmList\_MayNotReadFile** | 1 = The file must not be accessed, even if it is checked out and modified |
| **EdmList\_Nothing** | 0 = Default behavior |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)