<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmButtonState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmButtonState Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmButtonState Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

States of a toolbar button; used in calls to [IEdmAddInDrawButton5:DrawToolbarButton](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5~DrawToolbarButton.html), [IEdmCmdMgr5::AddToolbarImage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddToolbarImage.html), and [IEdmMenu5::GetButtonImages](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~GetButtonImages.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmButtonState     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmButtonState : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmButtonState : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **BState\_Cold** | 2 = Normal button display |
| **BState\_Disabled** | 3 = Button is disabled |
| **BState\_Hot** | 1 = Mouse cursor is hovering over the toolbar button; button should be highlighted |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)