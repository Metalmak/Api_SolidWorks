<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockBuildTreeFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmUnlockBuildTreeFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUnlockBuildTreeFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags used to control the creation of the check-in file tree created by the [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) interface. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmUnlockBuildTreeFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmUnlockBuildTreeFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmUnlockBuildTreeFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Eubtf\_ForceUnlock** | 32768 = Unlock the file even if it is not modified; use only in combination with Eubtf\_MayUnlock |
| **Eubtf\_MayUndoLock** | 2 = Support undo file check-out |
| **Eubtf\_MayUnlock** | 1 = Support file check-in |
| **Eubtf\_MayUnlockWithLatest** | 4096 = Check in latest version instead of cached version; use only in combination with Eubtf\_MayUnlock |
| **Eubtf\_MayUnlockWithoutOverwrite** | 16384 = Check in without version overwrite; use only in combination with Eubtf\_MayUnlock |
| **Eubtf\_NoCallbackDlgErrors** | 256 = Do not pass dialog box errors to the callback |
| **Eubtf\_NoRemoveLocalCopy** | 128 = Do not display the **Remove Local Copy** column in the dialog box |
| **Eubtf\_Nothing** | 0 = None of the other flags |
| **Eubtf\_RefreshFileListing** | 32 = Refresh the file listing in the File Explorer when the operation completes |
| **Eubtf\_SearchForDrawings** | 512 = Include drawings as sub-parent nodes |
| **Eubtf\_ShowCloseAfterCheckinOption** | 2048 = Display the **Reload or Close Files after Check In** dropdown on the Check In or Undo Check Out dialog box toolbar; this option permits the user to choose whether to close the files in SOLIDWORKS after the check-in operation has succeeded or reload them in SOLIDWORKS |
| **Eubtf\_ShowMultipleWarnings** | 8192 = Display Multiple Warnings link in warning column of dialog |
| **Eubtf\_SkipOpenFileChecks** | 1024 = Do not check whether files are open in another application |
| **Eubtf\_UndoLockDefault** | 4 = Make undo check-out the default operation |
| **Eubtf\_Warn\_UndoLockModifiedInCb** | 16 = Warn the caller of undo check-out of modified files via the callback interface |
| **Eubtf\_Warn\_UndoLockModifiedInDlg** | 8 = Show warning icon in the Undo Check Out dialog box for modified files marked for undo check-out |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)