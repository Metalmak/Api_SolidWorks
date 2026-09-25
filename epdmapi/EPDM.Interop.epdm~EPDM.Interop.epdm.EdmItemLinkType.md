<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemLinkType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmItemLinkType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmItemLinkType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of linked files to items.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmItemLinkType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmItemLinkType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmItemLinkType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmItemLnk\_Attachment** | 1 = Attachment links are referred to as static links in the user interface; a statically linked file does not drive the associated item; it is just an attachment |
| **EdmItemLnk\_Dynamic** | 0 = Dynamic links are referred to as auto-update links in the user interface in SOLIDWORKS PDM Professional 2010 and later; this means that some changes in the linked file automatically propagates to the item |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[EdmGenItemInfo Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo.html)