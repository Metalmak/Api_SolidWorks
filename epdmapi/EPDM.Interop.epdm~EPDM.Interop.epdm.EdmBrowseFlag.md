<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrowseFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmBrowseFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBrowseFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Browse options used in calls to [IEdmVault5::BrowseForFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~BrowseForFile.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmBrowseFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmBrowseFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmBrowseFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmBws\_ForOpen** | 0 = Display the Open dialog box |
| **EdmBws\_ForSave** | 1 = Display a Save As dialog box |
| **EdmBws\_Help** | 32 = Display **Help** in the dialog box |
| **EdmBws\_PermitExternalFiles** | 16 = Permit the user to select files that are outside the file vault folder tree |
| **EdmBws\_PermitLocalFiles** | 4 = Permit the user to select files that are inside the file vault folder tree, but not checked in to the vault |
| **EdmBws\_PermitMultipleSel** | 2 = Permit the user to select more than one file |
| **EdmBws\_PermitVaultFiles** | 8 = Permit the user to select files that are part of the file vault |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)