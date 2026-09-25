<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmSearch5 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmSearch5 Interface |

The following tables list the members exposed by [IEdmSearch5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [FileName](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~FileName.html) | Gets or sets the name of the file or folder for which to search. |
| ![ Property](dotnetimages/Property.gif) | [FindFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~FindFiles.html) | Gets or sets whether to return files in the search. |
| ![ Property](dotnetimages/Property.gif) | [FindFolders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~FindFolders.html) | Gets or sets whether to return folders in the search. |
| ![ Property](dotnetimages/Property.gif) | [FindHistoricStates](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~FindHistoricStates.html) | Gets or sets whether to find all files that have ever been in the state specified by [IEdmSearch5::State](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~State.html). |
| ![ Property](dotnetimages/Property.gif) | [FindLockedFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~FindLockedFiles.html) | Gets or sets whether to include checked-out files in the search result. |
| ![ Property](dotnetimages/Property.gif) | [FindUnlockedFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~FindUnlockedFiles.html) | Gets or sets whether to include checked-in files in the search result. |
| ![ Property](dotnetimages/Property.gif) | [Recursive](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~Recursive.html) | Gets or sets whether to search recursively in subfolders. |
| ![ Property](dotnetimages/Property.gif) | [StartFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~StartFolderID.html) | Gets or sets the ID of the folder in which to search. |
| ![ Property](dotnetimages/Property.gif) | [State](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~State.html) | Gets or sets the ID or name of the workflow state in which to search. |
| ![ Property](dotnetimages/Property.gif) | [VersionComment](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~VersionComment.html) | Gets or sets the version comment substring for which to search. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddVariable](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~AddVariable.html) | Obsolete. Superseded by [IEdmSearch8::AddVariable2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8~AddVariable2.html). |
| ![ Method](dotnetimages/Method.gif) | [Clear](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~Clear.html) | Resets all search properties to their default values |
| ![ Method](dotnetimages/Method.gif) | [GetFirstResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~GetFirstResult.html) | Gets the first file or folder that matches the search criteria. |
| ![ Method](dotnetimages/Method.gif) | [GetNextResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~GetNextResult.html) | Gets the next file or folder that matches the search criteria. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)