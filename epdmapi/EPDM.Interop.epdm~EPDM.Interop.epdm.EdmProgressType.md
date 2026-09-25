<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmProgressType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmProgressType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmProgressType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of progress bars that are affected by certain operations.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmProgressType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmProgressType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmProgressType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Ept\_FileTransfer** | 2 = Progress bar for copying the data of a single file |
| **Ept\_Operation** | 1 = Progress bar for the entire operation |
| **Ept\_UpdateReference** | 3 = Progress bar for updating file references |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmGetOpCallback::ProgressBegin Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ProgressBegin.html)

[IEdmGetOpCallback::ProgressEnd Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ProgressEnd.html)

[IEdmGetOpCallback::ProgressStep Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ProgressStep.html)

[IEdmUnlockOpCallback::ProgressBegin Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressBegin.html)

[IEdmUnlockOpCallback::ProgressEnd Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressEnd.html)

[IEdmUnlockOpCallback::ProgressStep Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressStep.html)

[IEdmUnlockOpCallback::ProgressStepEvent Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressStepEvent.html)