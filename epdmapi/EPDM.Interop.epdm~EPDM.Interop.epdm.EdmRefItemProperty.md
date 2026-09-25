<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefItemProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmRefItemProperty Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRefItemProperty Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of property that can be accessed in [IEdmRefItem](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html) objects via [IEdmRefItem::GetProperty](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem~GetProperty.html) and [IEdmRefItem::SetProperty](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem~SetProperty.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmRefItemProperty     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmRefItemProperty : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmRefItemProperty : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmrip\_CheckAdd** | 27 = R+W; Boolean; add file? |
| **Edmrip\_CheckChangeState** | 28 = R+W; Boolean; change the state of the file? |
| **Edmrip\_CheckCopy** | 24 = R+W; Boolean; copy file? |
| **Edmrip\_CheckGet** | 20 = R+W; Boolean; retrieve file? |
| **Edmrip\_CheckHasBlockingWarning** | 30 = R+W; Boolean; file has blocking warning? |
| **Edmrip\_CheckIncRev** | 21 = R+W; Boolean; increment revision? |
| **Edmrip\_CheckKeepLocked** | 19 = R+W; Boolean; keep check-out state after check in? |
| **Edmrip\_CheckLock** | 17 = R+W; Boolean; check out file? |
| **Edmrip\_CheckOverwriteLatestVersion** | 29 = R+W; Boolean; overwrite the latest version of the file with the new changes instead of creating a new version? |
| **Edmrip\_CheckRemoveLocal** | 23 = R+W; Boolean; Check In container; remove local file copy after check in? |
| **Edmrip\_CheckUndoLock** | 22 = R+W; Boolean; Check In container; remove check-out state without producing a new version? |
| **Edmrip\_CheckUnlock** | 18 = R+W; Boolean; Check In container; check in file? |
| **Edmrip\_FileName** | 2 = R; string; All container; filename |
| **Edmrip\_FoundPath** | 7 = R; string; Check In container; file system path to folder where file is found |
| **Edmrip\_ID** | 0 = R; string; All container; unique ID of the item in the container |
| **Edmrip\_IncludedAs** | 6 = R; string; Check In container; include path used to reference this file |
| **Edmrip\_LockComputer** | 4 = R; string; Check In container; name of computer where file is checked out |
| **Edmrip\_LockPath** | 3 = R; string; Check In container; file system path to folder where file is checked out |
| **Edmrip\_LockUser** | 5 = R; string; Check In container; name of user who checked out file |
| **Edmrip\_RefName** | 1 = R; string; All container; name of file reference; does not have to be the filename |
| **Edmrip\_RevisionLatest** | 15 = R; string; current revision number of file |
| **Edmrip\_RevisionNew** | 16 = R; string; next revision number of file |
| **Edmrip\_ShowMultipleWarnings** | 31 = R+W; Boolean; display the **Multiple Warnings** link in the command dialog box's warning column? |
| **Edmrip\_Size** | 33 = R; integer; file size |
| **Edmrip\_StatusHresult** | 25 = R; HRESULT; All container; binary error code for this item |
| **Edmrip\_StatusText** | 26 = R; string; All container; error code |
| **Edmrip\_TransitionID** | 34 = R; integer; Transition ID returned with change state operation |
| **Edmrip\_Type** | 32 = R; integer; Check In container; type of file: 1=normal, 2=virtual, 3=BOM, 4=item, 5=cutlist, 6=toolbox part |
| **Edmrip\_VersionAttached** | 11 = R; integer; Check In container; version that was referenced before check in |
| **Edmrip\_VersionLatest** | 9 = R; integer; Check In container; latest version of the file |
| **Edmrip\_VersionLocal** | 8 = R; integer; Check In container; version of file copy on the local disk |
| **Edmrip\_VersionNew** | 10 = R; integer; Check In container; next version of the file |
| **Edmrip\_VersionNewAttached** | 12 = R; integer; Check In container; version that will be referenced after check in |
| **Edmrip\_WorkflowStateIcon** | 14 = R; string; Check In container; name of the file's current workflow state icon |
| **Edmrip\_WorkflowStateName** | 13 = R; string; Check In container; name of the file's current workflow state |

# ![](dotnetimages/collapse.gif)Remarks

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)