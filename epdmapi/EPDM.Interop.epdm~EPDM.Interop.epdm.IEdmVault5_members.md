<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmVault5 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmVault5 Interface |

The following tables list the members exposed by [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CommandID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~CommandID.html) | Gets the command ID count. |
| ![ Property](dotnetimages/Property.gif) | [IsLoggedIn](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~IsLoggedIn.html) | Gets whether you are logged in to this vault. |
| ![ Property](dotnetimages/Property.gif) | [Language](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Language.html) | Gets the language used by the SOLIDWORKS PDM Professional client. |
| ![ Property](dotnetimages/Property.gif) | [Name](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Name.html) | Gets the name of this vault. |
| ![ Property](dotnetimages/Property.gif) | [RootFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~RootFolder.html) | Gets the root folder of this vault. |
| ![ Property](dotnetimages/Property.gif) | [RootFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~RootFolderID.html) | Gets the database ID of the root folder of this vault. |
| ![ Property](dotnetimages/Property.gif) | [RootFolderPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~RootFolderPath.html) | Gets the file system path to the root folder of this vault. |
| ![ Property](dotnetimages/Property.gif) | [SilentMode](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~SilentMode.html) | Gets whether the add-in is running in silent mode. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [BrowseForFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~BrowseForFile.html) | Displays an Open or Save As dialog box in which the user can click one or more files. |
| ![ Method](dotnetimages/Method.gif) | [BrowseForFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~BrowseForFolder.html) | Obsolete. Superseded by [IEdmVault11::BrowseForFolder2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~BrowseForFolder2.html). |
| ![ Method](dotnetimages/Method.gif) | [CreatePluginMenu](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~CreatePluginMenu.html) | Obsolete. Superseded by [IEdmVault12::CreatePluginMenu2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12~CreatePluginMenu2.html). |
| ![ Method](dotnetimages/Method.gif) | [CreateSearch](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~CreateSearch.html) | Obsolete. Superseded by [IEdmVault21::CreateSearch2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault21~CreateSearch2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetDictionary](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetDictionary.html) | Gets or creates the specified dictionary. |
| ![ Method](dotnetimages/Method.gif) | [GetErrorString](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetErrorString.html) | Gets the name and description for the specified error code returned by one of SOLIDWORKS PDM Professional's API methods. |
| ![ Method](dotnetimages/Method.gif) | [GetFileFromPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetFileFromPath.html) | Gets an interface to the file with the specified file system path. |
| ![ Method](dotnetimages/Method.gif) | [GetFolderFromPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetFolderFromPath.html) | Gets an interface to a folder on the specified file system path. |
| ![ Method](dotnetimages/Method.gif) | [GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html) | Gets an interface to a SOLIDWORKS PDM Professional object of the specified type and having the specified ID. |
| ![ Method](dotnetimages/Method.gif) | [GetVaultNameFromPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetVaultNameFromPath.html) | Gets the name of the vault where the specified file or folder resides. |
| ![ Method](dotnetimages/Method.gif) | [GetVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetVersion.html) | Gets the version of SOLIDWORKS PDM Professional that is installed on this machine. |
| ![ Method](dotnetimages/Method.gif) | [Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) | Logs in to the specified vault using the specified user name and password. |
| ![ Method](dotnetimages/Method.gif) | [LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html) | Logs in to the specified vault. |
| ![ Method](dotnetimages/Method.gif) | [MsgBox](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~MsgBox.html) | Displays a message box to the user. |
| ![ Method](dotnetimages/Method.gif) | [RefreshFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~RefreshFolder.html) | Refreshes the file listing in the specified folder. |
| ![ Method](dotnetimages/Method.gif) | [SetAddInWnd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~SetAddInWnd.html) | Obsolete. See [Keeping Add-in Windows in the Foreground](KeepWindowInfront.htm). |
| ![ Method](dotnetimages/Method.gif) | [VerifyVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~VerifyVersion.html) | Verifies that the installed SOLIDWORKS PDM Professional is at the specified version level or higher. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)