<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmBomFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBomFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Bill of Materials options used in calls to [IEdmFile7::GetComputedBOM](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7~GetComputedBOM.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmBomFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmBomFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmBomFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmBf\_AsBuilt** | 1 = Include as-built referenced files, i.e., the versions which were present in the cache when the parent file was checked in |
| **EdmBf\_ShowSelected** | 2 = Include the selected file in the Bill of Materials; if this flag is not set, only its children are included |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)