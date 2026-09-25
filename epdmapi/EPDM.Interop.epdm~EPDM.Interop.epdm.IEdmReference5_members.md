<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmReference5 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmReference5 Interface |

The following tables list the members exposed by [IEdmReference5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [File](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~File.html) | Gets the file. |
| ![ Property](dotnetimages/Property.gif) | [FileID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~FileID.html) | Gets the ID of the file. |
| ![ Property](dotnetimages/Property.gif) | [Folder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~Folder.html) | Gets the file's parent folder. |
| ![ Property](dotnetimages/Property.gif) | [FolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~FolderID.html) | Gets the ID of the file's parent folder. |
| ![ Property](dotnetimages/Property.gif) | [FoundPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~FoundPath.html) | Gets the file system path where the file was found. |
| ![ Property](dotnetimages/Property.gif) | [IsLocked](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~IsLocked.html) | Gets whether the file is checked out. |
| ![ Property](dotnetimages/Property.gif) | [LockedByUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~LockedByUser.html) | Gets the the user who checked out the file. |
| ![ Property](dotnetimages/Property.gif) | [LockedInFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~LockedInFolder.html) | Gets the folder in which the file is checked out. |
| ![ Property](dotnetimages/Property.gif) | [LockedOnComputer](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~LockedOnComputer.html) | Gets the name of the computer on which the file is checked out. |
| ![ Property](dotnetimages/Property.gif) | [LockPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~LockPath.html) | Gets the file's check-out path. |
| ![ Property](dotnetimages/Property.gif) | [Name](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~Name.html) | Gets the name of the file. |
| ![ Property](dotnetimages/Property.gif) | [ReferencedAs](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~ReferencedAs.html) | Gets how the file is included by the referencing file. |
| ![ Property](dotnetimages/Property.gif) | [VersionLocal](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~VersionLocal.html) | Gets the local version number of the file. |
| ![ Property](dotnetimages/Property.gif) | [VersionRef](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~VersionRef.html) | Gets the referenced version number of the file. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetCustomData](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetCustomData.html) | Gets data stored with [IEdmReference5::SetCustomData](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~SetCustomData.html) in this file reference. |
| ![ Method](dotnetimages/Method.gif) | [GetFirstChildPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetFirstChildPosition.html) | Obsolete. Superseded by [IEdmReference7::GetFirstChildPosition2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7~GetFirstChildPosition2.html) |
| ![ Method](dotnetimages/Method.gif) | [GetFirstParentPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetFirstParentPosition.html) | Obsolete. Superseded by [IEdmReference7::GetFirstParentPosition2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7~GetFirstParentPosition2.html) |
| ![ Method](dotnetimages/Method.gif) | [GetNextChild](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetNextChild.html) | Enumerates the files referenced by this file. |
| ![ Method](dotnetimages/Method.gif) | [GetNextParent](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetNextParent.html) | Enumerates the files referencing this file. |
| ![ Method](dotnetimages/Method.gif) | [SetCustomData](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~SetCustomData.html) | Stores an arbitrary piece of data in this object. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7.html)

[IEdmReference8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference8.html)

[IEdmReference9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference9.html)