<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupDataFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmGroupDataFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGroupDataFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options specified in [EdmGroupData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData.html) used by [IEdmUserMgr6::AddGroups](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6~AddGroups.html) to create new groups.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmGroupDataFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmGroupDataFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmGroupDataFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmgdf\_ForceAdd** | 4 = Add this group even if validation of the other groups in the array failed |
| **Edmgdf\_GetInterface** | 1 = Retrieve the interface of the group and return it in [EdmGroupData::mpoGroup](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData.html) |
| **Edmgdf\_Nothing** | 0 = No options |
| **Edmgdf\_Replace** | 2 = Replace the existing group |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)