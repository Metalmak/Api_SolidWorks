<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockEvent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmUnlockEvent Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUnlockEvent Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of check-in command passed to the [IEdmUnlockOpCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html) interface to notify the caller about what is happening while checking in files with the [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) interface.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmUnlockEvent     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmUnlockEvent : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmUnlockEvent : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Euev\_CompressingTree** | 3 = Check-in command is compressing the reference tree |
| **Euev\_ReadingFileRefs** | 1 = Check-in command is reading external references from the file |
| **Euev\_UnlockFile** | 2 = Check-in command is checking in a file |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)