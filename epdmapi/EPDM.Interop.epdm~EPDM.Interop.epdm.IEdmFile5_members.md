<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmFile5 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmFile5 Interface |

The following tables list the members exposed by [IEdmFile5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CurrentRevision](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~CurrentRevision.html) | Gets the file's current revision. |
| ![ Property](dotnetimages/Property.gif) | [CurrentState](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~CurrentState.html) | Gets the file's current workflow state. |
| ![ Property](dotnetimages/Property.gif) | [CurrentVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~CurrentVersion.html) | Gets the file's current version number. |
| ![ Property](dotnetimages/Property.gif) | [ID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~ID.html) | Gets the database ID of this file. |
| ![ Property](dotnetimages/Property.gif) | [IsLocked](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~IsLocked.html) | Gets whether the file is checked out. |
| ![ Property](dotnetimages/Property.gif) | [LockedByUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockedByUser.html) | Gets the user who has the file checked out. |
| ![ Property](dotnetimages/Property.gif) | [LockedByUserID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockedByUserID.html) | Gets the ID of the user who has the file checked out. |
| ![ Property](dotnetimages/Property.gif) | [LockedInFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockedInFolder.html) | Gets the folder in which this file is checked out. |
| ![ Property](dotnetimages/Property.gif) | [LockedInFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockedInFolderID.html) | Gets the ID of the folder in which this file is checked out. |
| ![ Property](dotnetimages/Property.gif) | [LockedOnComputer](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockedOnComputer.html) | Gets the name of the computer to which the file is checked out. |
| ![ Property](dotnetimages/Property.gif) | [LockPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockPath.html) | Gets the full path to the checked-out file. |
| ![ Property](dotnetimages/Property.gif) | [Name](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~Name.html) | Gets the name of the file. |
| ![ Property](dotnetimages/Property.gif) | [ObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~ObjectType.html) | Gets the type of object. |
| ![ Property](dotnetimages/Property.gif) | [Vault](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~Vault.html) | Gets the file vault to which this file belongs. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [ChangeState](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~ChangeState.html) | Obsolete. Superseded by [IEdmFile10::ChangeState2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile10~ChangeState2.html) |
| ![ Method](dotnetimages/Method.gif) | [GetConfigurations](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetConfigurations.html) | Gets a list of names of the configurations for the specified version of this file. |
| ![ Method](dotnetimages/Method.gif) | [GetEnumeratorVariable](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetEnumeratorVariable.html) | Gets an interface to this file's data card variables. |
| ![ Method](dotnetimages/Method.gif) | [GetFileCopy](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFileCopy.html) | Gets a copy of the file with the specified version from the archive and deposits it in the specified location. |
| ![ Method](dotnetimages/Method.gif) | [GetFirstFolderPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFirstFolderPosition.html) | Starts an enumeration of the parent folders of this file. |
| ![ Method](dotnetimages/Method.gif) | [GetLocalFileDate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalFileDate.html) | Gets the date and timestamp of a local copy of this file. |
| ![ Method](dotnetimages/Method.gif) | [GetLocalFileSize](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalFileSize.html) | Obsolete. Superseded by [IEdmFile9::GetLocalFileSize2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile9~GetLocalFileSize2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetLocalPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalPath.html) | Gets the full path to this file in the specified parent folder. |
| ![ Method](dotnetimages/Method.gif) | [GetLocalRevisionName](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalRevisionName.html) | Gets the revision name of the local copy of this file. |
| ![ Method](dotnetimages/Method.gif) | [GetLocalVersionNo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalVersionNo.html) | Obsolete. Superseded by [IEdmFile12::GetLocalVersionNo2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile12~GetLocalVersionNo2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetNextFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetNextFolder.html) | Gets the next parent folder of this file. |
| ![ Method](dotnetimages/Method.gif) | [GetReferenceTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetReferenceTree.html) | Gets an interface to the files that reference or are referenced by this file. |
| ![ Method](dotnetimages/Method.gif) | [GetRevisionGeneratorInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetRevisionGeneratorInfo.html) | Gets information about this file for the revision generator. |
| ![ Method](dotnetimages/Method.gif) | [IncrementRevision](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~IncrementRevision.html) | Creates a new revision of this file. |
| ![ Method](dotnetimages/Method.gif) | [IsKindOf](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~IsKindOf.html) | Checks whether the object is of a certain type. |
| ![ Method](dotnetimages/Method.gif) | [LockFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockFile.html) | Checks out this file from the vault to which the user is currently logged in. |
| ![ Method](dotnetimages/Method.gif) | [Refresh](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~Refresh.html) | Refreshes the file. |
| ![ Method](dotnetimages/Method.gif) | [Rename](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~Rename.html) | Obsolete. Superseded by [IEdmFile6::RenameEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6~RenameEx.html). |
| ![ Method](dotnetimages/Method.gif) | [UndoLockFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UndoLockFile.html) | Removes the check-out of a file without saving changes to the archive. |
| ![ Method](dotnetimages/Method.gif) | [UnlockFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UnlockFile.html) | Checks in this file. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)