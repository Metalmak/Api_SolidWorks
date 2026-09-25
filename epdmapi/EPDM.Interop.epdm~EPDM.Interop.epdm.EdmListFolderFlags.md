<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFolderFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmListFolderFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmListFolderFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags used in calls to [IEdmBatchListing::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~AddFolder.html) to tell how to add the folder to the list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmListFolderFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmListFolderFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmListFolderFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmListFolder\_Nothing** | 0 = None of the other values |
| **EdmListFolder\_Recursive** | 1 = Add the files inside the folder instead of adding the folder itself to the list; the files in any subfolders are added recursively |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)