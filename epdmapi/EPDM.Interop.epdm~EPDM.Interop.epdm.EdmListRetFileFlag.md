<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListRetFileFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmListRetFileFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmListRetFileFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags returned in an [IEdmBatchListing](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html) column if you specify column type [EdmCol\_EdmListRetFileFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmColType.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmListRetFileFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmListRetFileFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmListRetFileFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmLstRet\_Drawing** | 1 = It is a backwards drawing reference (i.e., it displayed as blue links in Enterprise's command dialog boxes) |
| **EdmLstRet\_InternalComponent** | 2 = Internal SOLIDWORKS part, cut list, etc.; i.e., it is not a physical file |
| **EdmLstRet\_Nothing** | 0 = It is an ordinary system file |
| **EdmLstRet\_ToolboxPart** | 4 = This is a part file from the Toolbox library |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmBatchListing2::CreateListEx Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing2~CreateListEx.html)