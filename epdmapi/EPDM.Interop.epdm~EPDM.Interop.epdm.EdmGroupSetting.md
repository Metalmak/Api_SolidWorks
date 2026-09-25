<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupSetting.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmGroupSetting Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGroupSetting Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

User group settings used by [IEdmUserGroup9::SetSettingsVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup9~SetSettingsVar.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmGroupSetting     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmGroupSetting : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmGroupSetting : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmGSv\_AutoDelete** | 9 = Whether to automatically delete local read-only files that are not part of the vault; 1 = true, 0 = false; this setting corresonds to the "Automatically delete local read-only files that are not part of the file vault" checkbox on the Explorer tab on the Settings dialog that appears when you click "Settings" on the Properties dialog of a group in the Admin Tool |
| **EdmGSv\_AutoGetLatest** | 11 = Whether to always work with the latest version of files; 1 = true, 0 = false; this setting corresponds to the "Always work with latest version of files" checkbox on the Reference Dialog tab on the Settings dialog that appears when you click "Settings" on the Properties dialog of a group in the Admin Tool |
| **EdmGSv\_AutoGetLatestRefs** | 43 = Whether to auto-select reference files to get latest when checking out; 1 = true, 0 = false; this setting corresponds to the "Auto select reference files to get latest when checking out" checkbox on the Reference Dialog tab on the Settings dialog that appears when you click "Settings" on the Properties dialog of a group in the Admin Tool |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)