<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetCmdFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmGetCmdFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGetCmdFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options for retrieving files from the vault used in calls to [IEdmBatchGet::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~CreateTree.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmGetCmdFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmGetCmdFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmGetCmdFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Egcf\_AsBuilt** | 1 = Use the same versions of referenced files that were used when the referencing file was checked in; if this bit is not set, the latest versions of referenced files are used |
| **Egcf\_AsBuiltNotDefault** | 128 = Use the as-built versions when creating the tree |
| **Egcf\_ForPreview** | 16 = Only retrieve referenced files that are needed by the preview when retrieving the referencing file; skip caching referenced files |
| **Egcf\_ForViewer** | 8192 = Only retrieve referenced files that are needed by the viewer when retrieving the referencing file; skip caching referenced files |
| **Egcf\_IncludeAutoCacheFiles** | 2048 = Selects the Check Out dialog box Get checkbox for the latest version if the referenced file is not in the local cache |
| **Egcf\_Lock** | 2 = Check out the files instead of just retrieving them |
| **Egcf\_LockNoLclCopyFiles** | 1024 = Locks the local referenced files if a local cache is not present |
| **Egcf\_LockReferencedFilesToo** | 64 = Check out files referenced by the checked-out file |
| **Egcf\_Nothing** | 0 = No options |
| **Egcf\_RefreshFileListing** | 32 = Refresh file listing in File Explorer after files have been checked out |
| **Egcf\_RollbackTree** | 4096 = Provide the ability to roll back files in the dialog |
| **Egcf\_SingleFileRollback** | 16384 = Roll back one file |
| **Egcf\_SkipExisting** | 8 = Do not retrieve files that already exist in the local cache |
| **Egcf\_SkipLockRefFiles** | 512 = Skips checking of lock file references |
| **Egcf\_SkipOpenFileChecks** | 256 = Skips checking whether the file is open in another application |
| **Egcf\_SkipUnlockedWritable** | 4 = Do not retrieve files that are writable and not checked out |
| **Egcf\_XrefsOpenCheck** | 32768 = Check whether cross-reference files are open in another application |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)