<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmInstallFileFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmInstallFileFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmInstallFileFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Operations used in calls to [IEdmVault12::InstallFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12~InstallFile.html) to control the installation of data.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmInstallFileFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmInstallFileFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmInstallFileFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmIff\_Nothing** | 0 = Default operation |
| **EdmIff\_ReplaceDuplicates** | 1 = This flag is used for CEX-files when you want to replace duplicate objects in the vault; i.e., if you are importing a group named "ABC" and if there is already a different group named "ABC" in the vault, it will be silently replaced; the default behavior is not to replace duplicates |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)