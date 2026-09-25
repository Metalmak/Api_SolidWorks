<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmFolder5 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmFolder5 Interface |

The following tables list the members exposed by [IEdmFolder5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [ID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~ID.html) | Gets the database ID of this folder. |
| ![ Property](dotnetimages/Property.gif) | [LocalPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~LocalPath.html) | Gets the full file system path to this local folder. |
| ![ Property](dotnetimages/Property.gif) | [Name](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~Name.html) | Gets the name of the folder. |
| ![ Property](dotnetimages/Property.gif) | [ObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~ObjectType.html) | Gets the type of object. |
| ![ Property](dotnetimages/Property.gif) | [ParentFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~ParentFolder.html) | Gets the interface to the parent folder of this folder. |
| ![ Property](dotnetimages/Property.gif) | [Vault](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~Vault.html) | Gets the file vault to which this folder belongs. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFile.html) | Obsolete. Superseded by [IEdmFolder8::AddFile2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8~AddFile2.html) |
| ![ Method](dotnetimages/Method.gif) | [AddFileShared](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFileShared.html) | Shares a file in another folder with this folder. |
| ![ Method](dotnetimages/Method.gif) | [AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFolder.html) | Creates a subfolder in this folder. |
| ![ Method](dotnetimages/Method.gif) | [CopyFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CopyFile.html) | Obsolete. Superseded by [IEdmFolder8::CopyFile2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8~CopyFile2.html) |
| ![ Method](dotnetimages/Method.gif) | [CreateCardView](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateCardView.html) | Obsolete. Superseded by [IEdmFolder10::CreateCardView2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder10~CreateCardView2.html). |
| ![ Method](dotnetimages/Method.gif) | [CreateFolderPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateFolderPath.html) | Creates all subfolders in a path relative to this folder. |
| ![ Method](dotnetimages/Method.gif) | [CreateLabel](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateLabel.html) | Creates a label on this folder and its subfolders. |
| ![ Method](dotnetimages/Method.gif) | [DeleteFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFile.html) | Deletes a file having the specified ID from this folder. |
| ![ Method](dotnetimages/Method.gif) | [DeleteFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFolder.html) | Deletes the specified subfolder from this folder. |
| ![ Method](dotnetimages/Method.gif) | [GetCard](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetCard.html) | Gets the interface to a data card of a file of the specified file type or the interface to the data card of this folder. |
| ![ Method](dotnetimages/Method.gif) | [GetCardID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetCardID.html) | Gets the ID of the data card of a file with the specified extension or the ID of the data card of this folder. |
| ![ Method](dotnetimages/Method.gif) | [GetFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetFile.html) | Gets the interface to a file with the specified name in this folder. |
| ![ Method](dotnetimages/Method.gif) | [GetFirstFilePosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetFirstFilePosition.html) | Starts an enumeration of the files in this folder. |
| ![ Method](dotnetimages/Method.gif) | [GetFirstLabelPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetFirstLabelPosition.html) | Starts an enumeration of the labels in this folder. |
| ![ Method](dotnetimages/Method.gif) | [GetFirstSubFolderPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetFirstSubFolderPosition.html) | Starts an enumeration of the subfolders in this folder. |
| ![ Method](dotnetimages/Method.gif) | [GetNextFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetNextFile.html) | Gets the next file in the enumeration. |
| ![ Method](dotnetimages/Method.gif) | [GetNextLabel](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetNextLabel.html) | Gets the next label in the enumeration. |
| ![ Method](dotnetimages/Method.gif) | [GetNextSubFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetNextSubFolder.html) | Gets the next subfolder in the enumeration. |
| ![ Method](dotnetimages/Method.gif) | [GetSubFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetSubFolder.html) | Gets the interface to the subfolder with the specified name. |
| ![ Method](dotnetimages/Method.gif) | [HasRights](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRights.html) | Obsolete. Superseded by [IEdmFolder5::HasRightsEx.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRightsEx.html) |
| ![ Method](dotnetimages/Method.gif) | [HasRightsEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRightsEx.html) | Gets whether the user has the specified rights for the specified file in this folder. |
| ![ Method](dotnetimages/Method.gif) | [IsKindOf](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~IsKindOf.html) | Checks whether the object is of a certain type. |
| ![ Method](dotnetimages/Method.gif) | [Refresh](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~Refresh.html) | Refreshes the file listing for the folder. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)