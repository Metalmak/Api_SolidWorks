<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmUnlockFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUnlockFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags used in [IEdmFile5::UnlockFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UnlockFile.html) to control the behavior of the check-in operation. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmUnlockFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmUnlockFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmUnlockFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmUnlock\_FailOnRegenerationNeed** | 16 = Fail if the file needs to be regenerated in the CAD program   **NOTE**: Only files resaved in SOLIDWORKS 2009 or later can trigger this flag |
| **EdmUnlock\_ForceUnlock** | 256 = Unlock the file even if it is not modified |
| **EdmUnlock\_IgnoreCorruptFile** | 4 = Ignore files with file formats unrecognized by SOLIDWORKS PDM Professional; without this flag, SOLIDWORKS PDM Professional returns [E\_EDM\_INVALID\_FILE](ReturnCodes.htm) if it encounters a corrupt file or a file containing a newer format than SOLIDWORKS PDM Professional can handle |
| **EdmUnlock\_IgnoreReferences** | 128 = Silently unlock parent files without their references |
| **EdmUnlock\_IgnoreRefsNotLockedByCaller** | 32 = Ignore references not locked by caller |
| **EdmUnlock\_IgnoreRefsOutsideVault** | 8 = Ignore references to files outside the vault |
| **EdmUnlock\_KeepLocked** | 1 = Keep the file checked out after creating the new version in the archive |
| **EdmUnlock\_OverwriteLatestVersion** | 64 = Do not create a new version; overwrite the last version of the file with new changes |
| **EdmUnlock\_RemoveLocalCopy** | 2 = Remove the local copy of the file from the hard disk after the file has been checked in |
| **EdmUnlock\_Simple** | 0 = Check in the file using default behavior |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)