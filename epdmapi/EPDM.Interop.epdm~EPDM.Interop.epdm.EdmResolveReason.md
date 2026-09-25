<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmResolveReason.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmResolveReason Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmResolveReason Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of flags, which contain the reason for the function call, to pass to your implementation of [IEdmCallback6::Resolve](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6~Resolve.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmResolveReason     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmResolveReason : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmResolveReason : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmrr\_DstExists** | 1 = Destination file name is already used in the folder |
| **Edmrr\_DstExistsGlobal** | 64 = Destination file name is already used in the vault |
| **Edmrr\_FolderExists** | 32 = Folder with the same name exists |
| **Edmrr\_LockedByYouHere** | 2 = Destination (existing) file is checked out by the logged-in user |
| **Edmrr\_SameAsSource** | 4 = Source file and the destination file are the same |
| **Edmrr\_SerialNumber** | 16 = Source file contains serial number values |
| **Edmrr\_UniqueValues** | 8 = Source file contains unique, constrained, variable values that must be cleared on copy |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)