<!-- source: epdmapi/EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode.EdmResultErrorCodes_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmResultErrorCodes\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.EPDMResultCode Namespace](EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode_namespace.html) : EdmResultErrorCodes\_e Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Error codes. See [EdmResultSuccessCodes\_e](EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode.EdmResultSuccessCodes_e.html) for the success codes.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmResultErrorCodes_e     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmResultErrorCodes_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmResultErrorCodes_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **E\_EDM\_ADDIN\_CANT\_ACCESS\_REGISTRY** | 0x800402D8 = Cannot redirect registry to retrieve add-in class ID |
| **E\_EDM\_ADDIN\_CLSID\_ALREADY\_USED** | 0x800402CE = There is already an add-in using the CLSID that you are trying to add; class IDs must be unique |
| **E\_EDM\_ADDIN\_CLSID\_NOT\_FOUND** | 0x800402DA = The add-in registration succeeded, but the add-in's class ID could not be found in the registry |
| **E\_EDM\_ADDIN\_FILE\_NOT\_FOUND** | 0x800402D6 = The add-in file was not found |
| **E\_EDM\_ADDIN\_LOAD\_CONFLICT** | 0x800402DB = The add-in could not be loaded; this can happen if an attempt is made to register a new version of a .NET add-in that is already loaded; the situation can usually be resolved by closing the application and reattempting the operation |
| **E\_EDM\_ADDIN\_LOADCONFLICT** | 0x80040284 = An older version of the add-in is already loaded in memory; restart the program to load the new version of the add-in |
| **E\_EDM\_ADDIN\_NAME\_ALREADY\_USED** | 0x800402D1 = There is already an add-in with the same name as the one you are trying to add; the name must be unique |
| **E\_EDM\_ADDIN\_NOT\_COM\_DLL** | 0x800402D7 = The specified add-in file is not a COM DLL |
| **E\_EDM\_ADDIN\_NOT\_FOUND** | 0x800402CF = The add-in cannot be found in the vault |
| **E\_EDM\_ADDIN\_NOT\_MULTITHREADED** | 0x800402AF = An attempt was made to add an add-in that is not a multithreaded COM-server |
| **E\_EDM\_ADDIN\_UNSUPPORTED\_OS** | 0x800402DC = The add-in does not support the operating system; you cannot load an 64-bit add-in in 32-bit Windows |
| **E\_EDM\_ALIAS\_USED\_IN\_EXPORT\_SCRIPT** | 0x800402AC = The alias set cannot be deleted because it is used in a data export rule |
| **E\_EDM\_ALIAS\_USED\_IN\_IMPORT\_SCRIPT** | 0x800402AD = The alias set cannot be deleted because it is used in a data import rule |
| **E\_EDM\_ALL\_GROUPS\_NOT\_VALIDATED** | 0x80040298 = All groups were not validated |
| **E\_EDM\_ALL\_USERS\_NOT\_VALIDATED** | 0x80040289 = All users were not validated |
| **E\_EDM\_ALREADY\_INITIALIZED** | 0x8004021B = An attempt was made to initialize an object twice; you can only initialize an object one time |
| **E\_EDM\_ALREADY\_LOGGED\_IN** | 0x80040205 = You tried to log in twice |
| **E\_EDM\_ARCHIVE\_LOGIN\_FAILED** | 0x80040243 = Login failed because of an invalid user name or password |
| **E\_EDM\_ARCHIVE\_ROOT\_FOLDER\_DOES\_NOT\_EXIST** | 0x800402C7 = Specified archive server root folder does not exist |
| **E\_EDM\_ARCHIVE\_SERVER\_NOT\_FOUND** | 0x8004023F = The archive server is not found; try starting the archive server |
| **E\_EDM\_AUTO\_LOGGED\_OUT** | 0x80040280 = You have been inactive for too long and have been logged out |
| **E\_EDM\_BAD\_LENGTH** | 0x80040242 = The statement is out of bounds |
| **E\_EDM\_BOM\_NOT\_FOUND** | 0x800402A9 = The specified bill of materials could not be found |
| **E\_EDM\_BOM\_USED\_IN\_EXPORT\_SCRIPT** | 0x800402AB = The bill of materials cannot be deleted because it is used in a data export rule |
| **E\_EDM\_CANCELLED\_BY\_USER** | 0x80040226 = The operation was canceled by the user |
| **E\_EDM\_CANT\_MOVE\_FOLDER\_TO\_SUBFOLDER** | 0x8004029C = An attempt was made to move a folder to one of its subfolders |
| **E\_EDM\_CANT\_OPEN\_DATABASE** | 0x80040206 = Could not open database; this could happen if the network connection is broken or if the database has been removed |
| **E\_EDM\_CANT\_START\_EDMSERVER** | 0x8004025B = Could not start EdmServer.exe; please reinstall the program |
| **E\_EDM\_CARD\_NOT\_FOUND** | 0x8004027E = The specified card could not be found |
| **E\_EDM\_CARDLIST\_HAS\_NO\_NAME** | 0x800402E1 =  Not the latest version, when latest version is required |
| **E\_EDM\_CIRCULAR\_XREF** | 0x8004022F = Detected cyclic file reference |
| **E\_EDM\_COLD\_STORAGE\_SCHEMA\_NOT\_FOUND** | 0x80040275 = The cold storage schema with the specified name was not found |
| **E\_EDM\_COLD\_STORE\_SCHEMA\_EXISTS** | 0x80040277 = Saving the cold storage schema failed because the name is already used by another schema |
| **E\_EDM\_COLUMN\_VIEW\_NOT\_FOUND** | 0x80040290 = The column view cannot be found |
| **E\_EDM\_COMMENT\_NOT\_ENTERED** | 0x800402F4 = Comment not entered |
| **E\_EDM\_CONDITIONS\_NOT\_MET** | 0x80040233 = Conditions for transition were not met |
| **E\_EDM\_COPYTREE\_ZIP\_FAILED** | 0x800402FB = Failed to create ZIP file during the file copy operation |
| **E\_EDM\_COULD\_NOT\_CREATE\_LOCAL\_FOLDER** | 0x8004021E = Could not create the folder in the local cache; the folder name might contain invalid characters |
| **E\_EDM\_COULD\_NOT\_LAUNCH\_TASKS** | 0x800402CB = Cannot launch tasks with user interface in silent mode |
| **E\_EDM\_COULD\_NOT\_OPEN\_CLIPBOARD** | 0x8004027A = Could not open the clipboard |
| **E\_EDM\_DATABASE\_ACCESS** | 0x80040207 = Could not access the item in the database |
| **E\_EDM\_DATABASE\_ALREADY\_EXISTS** | 0x800402D0 = A database with the same name already exists on the server |
| **E\_EDM\_DATABASE\_LINK\_FAILURE** | 0x80040267 = A communication link failure occurred when accessing the database server; the database service might have been restarted, or the network might be down; please try the operation again and contact your system administrator if the problem persists |
| **E\_EDM\_DATASOURCE\_NOT\_FOUND** | 0x80040222 = The ODBC data source was not found |
| **E\_EDM\_DISABLED** | 0x8004023D = The command is disabled |
| **E\_EDM\_DISK\_FULL** | 0x80040239 = The disk is full |
| **E\_EDM\_DOCTYPE\_EXISTS** | 0x80040259 = A category with the specified name already exists |
| **E\_EDM\_DOCTYPE\_IN\_USE** | 0x80040258 = The category is currently associated with one or more documents and cannot be deleted |
| **E\_EDM\_DONTSETMODIFIED\_FLAG** | 0x800402E5 = Do not set the modified flag |
| **E\_EDM\_DOTNET\_REGISTRATION\_MODULE\_MISSING** | 0x800402D9 = The .NET registration module is missing |
| **E\_EDM\_DRAWING\_IN\_DETAILING\_MODE** | 0x80040306 = The drawing is in detailing mode |
| **E\_EDM\_DUPLICATE\_GROUP\_NAME** | 0x80040268 = Saving the user group failed because the group name is already used by another group |
| **E\_EDM\_DUPLICATE\_SEARCH\_FAVORITE\_NAME** | 0x8004024B = Could not save the search favorite with the specified name because the name is already used by another favorite and the names must be unique; if the other favorite is not visible in the program, it is probably because you do not have permission to see it |
| **E\_EDM\_EMPTY\_VALUE\_FIELD** | 0x80040301 = The value of one or more transiiton conditions cannot be empty |
| **E\_EDM\_END\_OF\_LIST** | 0x80040208 = You tried to get an element from a list where the cursor is off right |
| **E\_EDM\_END\_OF\_REV\_GEN\_LIST\_CONTINUE** | 0x80040232 = You have reached the end of the revision generator list; please contact your system administrator to add more revision-generator entries in the workflow editor |
| **E\_EDM\_END\_OF\_REV\_GEN\_LIST\_STOP** | 0x80040231 = You have reached the end of the revision generator list; please contact your system administrator to add more revision-generator entries in the workflow editor |
| **E\_EDM\_END\_OF\_SN\_FILE** | 0x8004023A = You have reached the end of the serial number file |
| **E\_EDM\_ERPMGR\_ALIAS\_DOES\_NOT\_EXIST** | 0x8004029D = The alias does not exist |
| **E\_EDM\_ERPMGR\_EXPORT\_SCRIPT\_NOT\_FOUND** | 0x800402A8 = The specified export rule could not be found |
| **E\_EDM\_ERPMGR\_IMPORTBATCH\_DOES\_NOT\_EXIST** | 0x8004029E = The data import batch does not exist |
| **E\_EDM\_ERPMGR\_IMPORTSCRIPT\_NAME\_ALREADY\_EXISTS** | 0x8004029F = The name of the data import rule is already used |
| **E\_EDM\_ERPMGR\_INVALID\_DATE\_FORMAT** | 0x800402A0 = The date format is invalid |
| **E\_EDM\_ERPMGR\_INVALID\_FILENAME** | 0x800402A1 = The file name is invalid |
| **E\_EDM\_ERPMGR\_ITEM\_NOT\_FOUND** | 0x800402A2 = The data import/export item was not found in the database |
| **E\_EDM\_ERPMGR\_VALUE\_TOO\_LONG** | 0x800402A3 = The value is too long |
| **E\_EDM\_ERPMGR\_VARALIASSET\_ALREADY\_EXISTS** | 0x800402A4 = The specified alias set already exists |
| **E\_EDM\_ERPMGR\_VARALIASSET\_DOES\_NOT\_EXIST** | 0x800402A5 = The specified variable alias set does not exist |
| **E\_EDM\_ERPMGR\_VARIABLE\_DOES\_NOT\_EXIST** | 0x800402A6 = The specified variable does not exist |
| **E\_EDM\_ERPMGR\_VARIABLENAME\_NOT\_UNIQUE** | 0x800402A7 = The variable name is not unique |
| **E\_EDM\_EXCLUDED\_FROM\_PREVIEW** | 0x8004023C = The file type is excluded from preview |
| **E\_EDM\_FILE\_ALREADY\_OPEN** | 0x80040281 = The file is already open |
| **E\_EDM\_FILE\_DELETED** | 0x8004026D = The file has been deleted |
| **E\_EDM\_FILE\_FORMAT\_UNSUPPORTED\_BY\_CONISIO\_VERSION** | 0x8004026A = The file format is not supported by your SOLIDWORKS PDM Professional license |
| **E\_EDM\_FILE\_IN\_COLDSTORAGE** | 0x80040278 = The file that you are trying to access is currently placed in cold storage and cannot be retrieved |
| **E\_EDM\_FILE\_IS\_LOCKED** | 0x80040211 = The operation is not permitted because the file is checked out |
| **E\_EDM\_FILE\_IS\_REFERENCED** | 0x8004022D = The file is referenced by another file |
| **E\_EDM\_FILE\_NAME\_NOT\_GLOBALLY\_UNIQUE** | 0x80040286 = The file name, which needs to be unique in the file vault, has been used before |
| **E\_EDM\_FILE\_NOT\_FOUND** | 0x80040213 = The file could not be found |
| **E\_EDM\_FILE\_NOT\_LOCKED\_BY\_YOU** | 0x80040210 = The file is not checked out by you, which is required by the operation |
| **E\_EDM\_FILE\_NOT\_OPEN** | 0x80040282 = The file is not open |
| **E\_EDM\_FILE\_NOT\_REGENERATED** | 0x800402B3 = The file is not rebuilt |
| **E\_EDM\_FILE\_SHARE\_ERROR** | 0x8004020B = An attempt was made to access a file that is exclusively opened by another application |
| **E\_EDM\_FILES\_WERE\_LOCKED** | 0x80040257 = One or more documents have been checked out; these files have been deselected; click **OK** again if you still want to perform the operation on the remaining files |
| **E\_EDM\_FOLDER\_NOT\_EMPTY** | 0x8004021F = The specified folder is not empty |
| **E\_EDM\_FOLDER\_NOT\_FOUND** | 0x80040214 = The folder could not be found |
| **E\_EDM\_GET\_EDMFORMATROUTER** | 0x8004027D = The file format plug-in routes the call onto another plug-in; the file format manager will query the interface for the IEdmFormatRouter code to figure out which plug-in to use |
| **E\_EDM\_GROUP\_NAME\_ALREADY\_EXISTS** | 0x80040297 = The group name already exists |
| **E\_EDM\_GROUP\_NAME\_NOT\_UNIQUE** | 0x80040295 = The group name is not unique in the specified array of groups |
| **E\_EDM\_GROUP\_NOT\_FOUND** | 0x800402D4 = The group could not be found |
| **E\_EDM\_HAS\_NO\_CARD** | 0x80040227 = The file does not have a file data card |
| **E\_EDM\_HAS\_NO\_PARENT** | 0x80040202 = The folder does not have a parent |
| **E\_EDM\_HAS\_NO\_PREVIEW** | 0x80040223 = The file does not have a preview bitmap |
| **E\_EDM\_INDEXER\_NOT\_STARTED** | 0x8004027F = Indexing has not been set up for this file vault |
| **E\_EDM\_INSUFFICIENT\_SQL\_PERMISSION** | 0x80040283 = The SQL server user account associated with the vault has insufficient privileges; the administrator can solve this by running the following command in the SQL Server Query Analyzer: GRANT VIEW SERVER STATE TO *user name* |
| **E\_EDM\_INVALID\_BOM** | 0x800402EA = Invalid BOM |
| **E\_EDM\_INVALID\_CATEGORY\_ID** | 0x80040263 = The specified category database ID is invalid |
| **E\_EDM\_INVALID\_COLUMN\_VIEW** | 0x80040291 = The column view is invalid |
| **E\_EDM\_INVALID\_COMPLETE\_NAME** | 0x8004028B = The complete name is invalid |
| **E\_EDM\_INVALID\_DATABASE\_NAME** | 0x800402C3 = The SQL database name is invalid |
| **E\_EDM\_INVALID\_DATE\_FORMAT\_CODE** | 0x800402C5 = The SQL date format code is invalid |
| **E\_EDM\_INVALID\_EMAIL** | 0x8004028C = The email is invalid |
| **E\_EDM\_INVALID\_FILE** | 0x80040229 = The file format is not recognized |
| **E\_EDM\_INVALID\_FILE\_ID** | 0x80040264 = The specified file ID is invalid |
| **E\_EDM\_INVALID\_GROUP\_DESCRIPTION** | 0x80040296 = The group description is invalid |
| **E\_EDM\_INVALID\_GROUP\_MEMBER\_ID** | 0x80040299 = A group member ID is invalid |
| **E\_EDM\_INVALID\_GROUP\_NAME** | 0x80040294 = The group name is invalid |
| **E\_EDM\_INVALID\_ID** | 0x80040241 = The supplied object ID is not valid |
| **E\_EDM\_INVALID\_INITIALS** | 0x8004028D = The initials are invalid |
| **E\_EDM\_INVALID\_NAME** | 0x8004021D = The file/key name was invalid |
| **E\_EDM\_INVALID\_OUTLOOK\_VERSION** | 0x800402E2 = The specified version of Microsoft Outlook is invalid |
| **E\_EDM\_INVALID\_PASSWORD** | 0x8004028F = The password is invalid |
| **E\_EDM\_INVALID\_QUERY** | 0x80040230 = The search query is invalid |
| **E\_EDM\_INVALID\_REVISION\_NUMBER** | 0x80040224 = Specified revision number is invalid |
| **E\_EDM\_INVALID\_REVISION\_NUMBER\_COMPONENT\_NAME** | 0x8004029B = The revision number component name is invalid |
| **E\_EDM\_INVALID\_REVISION\_NUMBER\_GENERATOR\_NAME** | 0x8004029A = The revision number generator name is invalid |
| **E\_EDM\_INVALID\_SERIAL\_NUMBER\_NAME** | 0x80040256 = Invalid serial number name |
| **E\_EDM\_INVALID\_TRANSITION\_WEB** | 0x80040274 = Could not change state because the transition would create a new document version, which is not supported by the web client |
| **E\_EDM\_INVALID\_TYPE** | 0x80040225 = The object has an invalid type for the specified operation |
| **E\_EDM\_INVALID\_USER\_DATA** | 0x8004028E = The user data string is invalid |
| **E\_EDM\_INVALID\_USER\_NAME** | 0x80040287 = The user name is invalid |
| **E\_EDM\_INVALID\_VAULT\_NAME** | 0x800402C2 = The vault name is invalid |
| **E\_EDM\_INVALID\_WORKFLOW\_ID** | 0x80040260 = The specified workflow database ID is invalid |
| **E\_EDM\_INVALID\_WORKFLOW\_STATE\_ID** | 0x80040262 = The specified workflow state database ID is invalid |
| **E\_EDM\_INVALID\_WORKFLOW\_TRANSITION\_ID** | 0x80040261 = The specified workflow transition database ID is invalid |
| **E\_EDM\_IO\_ERROR** | 0x80040228 = Error accessing the file |
| **E\_EDM\_KEY\_NOT\_FOUND** | 0x8004022B = The key you specified was not found in the collection |
| **E\_EDM\_LABEL\_ALREADY\_EXIST** | 0x80040302 = The label already exists |
| **E\_EDM\_LOCAL\_FILE\_NOT\_FOUND** | 0x80040285 = The file is not present in the file vault cache folder on the client computer |
| **E\_EDM\_LOCK\_ERRORS** | 0x80040266 = One or more documents could not be checked out |
| **E\_EDM\_LOCKED** | 0x800402B0 = The file is checked out |
| **E\_EDM\_LOCKED\_BY\_ANOTHER\_USER** | 0x80040212 = The file is checked out by another user |
| **E\_EDM\_LOCKED\_IN\_OTHER\_FOLDER** | 0x800402B0 = The file is checked out in another folder |
| **E\_EDM\_LOCKED\_ON\_OTHER\_COMPUTER** | 0x80040215 = The file is checked out on another computer |
| **E\_EDM\_LOGIN\_FAILED** | 0x80040200 = Login failed because of an invalid user name or password |
| **E\_EDM\_LOGIN\_LOCK** | 0x8004024E = The system is locked due to maintenance |
| **E\_EDM\_MAILSERVER\_NOT\_INSTALLED** | 0x80040235 =  SOLIDWORKS PDM Professional Database Server is not installed on the database server; please contact your system administrator for assistance |
| **E\_EDM\_MAPPING\_FOUND** | 0x8004020E = Could not remove the attribute class because it is used by a control in a file data card |
| **E\_EDM\_MISSING\_ATTRIBUTE** | 0x8004020C = An attempt was made to access an attribute that is not present in the file |
| **E\_EDM\_MISSING\_CONISIO\_MODULE** | 0x80040272 = A required SOLIDWORKS PDM Professional module is not installed |
| **E\_EDM\_MISSING\_LOCAL\_VIEW** | 0x800402D5 = The vault must have a local view |
| **E\_EDM\_MISSING\_MANDATORY\_VALUE** | 0x80040236 = An attempt was made to save an empty value for a mandatory variable |
| **E\_EDM\_MISSING\_PLUGIN\_COMPONENT** | 0x80040245 = The file format plug-in cannot handle this file because a component is missing |
| **E\_EDM\_MISSING\_PTID** | 0x8004025A = The registry variable PTID is missing; please reinstall the program |
| **E\_EDM\_MISSING\_SEARCH\_PROC** | 0x8004024F = The search card's stored procedure is missing in the database |
| **E\_EDM\_MISSING\_URL\_PARAM** | 0x8004026E = A required URL parameter is missing |
| **E\_EDM\_MISSING\_VIEW\_INFO** | 0x8004024C = Could not find registry information for this view; you might have to attach to this vault again to repair the registry |
| **E\_EDM\_MOVE\_FILE\_PERMISSION\_DENIED** | 0x800402E4 = The user does not have permission to move the file. |
| **E\_EDM\_NAME\_ALREADY\_EXISTS** | 0x8004020F = An attempt was made to create a new file or folder with the same name as an existing one |
| **E\_EDM\_NEED\_MIGRATING** | 0x80040249 = The file needs to be migrated for the operation to succeed |
| **E\_EDM\_NO\_ACTIVE\_COLDSTORAGE\_OPERATION** | 0x80040276 = There are currently no active cold storage operations belonging to the calling archive server |
| **E\_EDM\_NO\_DOCTYPE** | 0x8004025C = The document does not meet the conditions of any category |
| **E\_EDM\_NO\_MATCHING\_PLUGIN** | 0x8004022A = There is no matching plug-in |
| **E\_EDM\_NO\_REVISION\_GENERATOR** | 0x80040247 = The file is not connected to a revision generator |
| **E\_EDM\_NO\_REVISION\_ON\_REFERENCE** | 0x80040237 = Cannot set revision because not all referenced files have revisions on the attached versions |
| **E\_EDM\_NO\_SECPKG\_FOUND** | 0x80040254 = Could not negotiate a security package to use between the server and the client |
| **E\_EDM\_NO\_WORKFLOW** | 0x8004025D = The document does not meet the conditions of any workflow |
| **E\_EDM\_NOT\_A\_COM\_DLL** | 0x800402CC = The DLL is not a COM module |
| **E\_EDM\_NOT\_AN\_ADDIN\_DLL** | 0x800402CD = The DLL is not an SOLIDWORKS PDM Professional add-in; i.e., the [IEdmAddIn5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) interface is not implemented |
| **E\_EDM\_NOT\_INITIALIZED** | 0x80040201 = The program used an object without properly initializing it |
| **E\_EDM\_NOT\_LATEST\_VERSION** | 0x800402E0 = Item must be checked out to perform this operation |
| **E\_EDM\_NOT\_LOGGED\_IN** | 0x80040204 = You have not logged into the file vault |
| **E\_EDM\_NOT\_POWER\_USER** | 0x80040246 = You are not logged in on Windows as a Power User or Administrator, which is required to run SOLIDWORKS PDM Professional |
| **E\_EDM\_NULL\_VALUE** | 0x80040240 = A null value was returned where it was not expected |
| **E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN** | 0x8004021A = The operation was not permitted by one of the installed add-ins |
| **E\_EDM\_OPERATION\_UNSUPPORTED\_BY\_CONISIO\_VERSION** | 0x8004026B = The operation is not supported by your SOLIDWORKS PDM Professional license |
| **E\_EDM\_PARENT\_LOCKED\_ELSEWHERE** | 0x800402B1 = The file is referenced by a file that is checked out on another computer |
| **E\_EDM\_PARENT\_LOCKED\_ELSEWHERE\_WITHFILE** | 0x80040300 = The file is referenced by a file, *file\_name*, that is checked out on another computer |
| **E\_EDM\_PASSWORD\_NOT\_EMPTY** | 0x80040293 = The current login type does not allow passwords to be set |
| **E\_EDM\_PATH\_TOO\_LONG** | 0x80040271 = The path is too long |
| **E\_EDM\_PERMISSION\_DENIED** | 0x80040203 = You do not have permission to perform this action |
| **E\_EDM\_PICTURE\_TOO\_BIG** | 0x800402E3 = The specified image is too big |
| **E\_EDM\_PREVIEW\_NOT\_AVAILABLE** | 0x800402BF = Preview is not available |
| **E\_EDM\_PRODUCT\_TIMEOUT** | 0x800402D2 = Your version of SOLIDWORKS PDM Professional has expired; contact your SOLIDWORKS representative for a newer version |
| **E\_EDM\_PROGRAM\_VERSION\_MISMATCH** | 0x80040270 = The server and client are not of the same version |
| **E\_EDM\_RCE\_ERROR** | 0x80040209 = Error accessing the revision management system; check your network connection |
| **E\_EDM\_REFERENCE\_EXISTS** | 0x8004027B = The reference already exists |
| **E\_EDM\_REVGEN\_EXISTS** | 0x8004025E = A revision number component with the specified name already exists |
| **E\_EDM\_REVGENERATOR\_IN\_USE** | 0x80040250 = The revision number component is currently being used by one or more revision numbers and cannot be deleted |
| **E\_EDM\_REVISION\_CHANGED** | 0x80040253 = The revision number has been changed by another user |
| **E\_EDM\_REVISION\_NO\_VERSION** | 0x80040251 = An attempt was made to set a revision on a version newer than the documents latest version |
| **E\_EDM\_REVISION\_ON\_OLD\_VERSION** | 0x80040238 = Cannot set revision on old version |
| **E\_EDM\_REVNUM\_EXISTS** | 0x8004025F = A revision number with the specified name already exists |
| **E\_EDM\_REVNUMBER\_IN\_USE** | 0x80040255 = The revision number is currently associated with one or more states and cannot be deleted |
| **E\_EDM\_ROLLBACK\_ERRORS** | 0x800402F7 = Rollback errors |
| **E\_EDM\_ROLLBACK\_FOLDER** | 0x800402F8 |
| **E\_EDM\_ROLLBACK\_PAST\_COLDSTORED** | 0x80040279 = The rollback operation cannot be performed because one of the versions that you are trying to remove is placed in cold storage |
| **E\_EDM\_SERIAL\_NUMBER\_NAME\_ALREADY\_EXISTS** | 0x800402AE = The serial number name is already in use |
| **E\_EDM\_SERNO\_USED\_AS\_ITEM\_GEN** | 0x800402C0 = The serial number cannot be deleted because it is used as an item number generator |
| **E\_EDM\_SERVER\_NOT\_FOUND** | 0x80040220 = The server was not found |
| **E\_EDM\_SKIP\_FILE** | 0x80040273 = The user selected to skip processing of the current file and go on to the next one |
| **E\_EDM\_SN\_FILE\_NOT\_FOUND** | 0x8004023B = Serial number file or add-in could not be found |
| **E\_EDM\_SN\_TYPE\_OBSOLETE** | 0x800402B2 = Serial numbers read from files are no longer supported; please open the serial number in the Administration tool and resave it as a list serial number |
| **E\_EDM\_SQLSERVER\_CANNOT\_CONNECT** | 0x800402C6 = Cannot connect to specified SQL server |
| **E\_EDM\_SQLSERVER\_LOGIN\_FAILED** | 0x800402C4 = Login failed because of an invalid SQL user name or password |
| **E\_EDM\_SQLSERVER\_UNSUPPORTED\_VERSION** | 0x8004027C = The SQL Server version is not supported by SOLIDWORKS PDM Professional; supported versions are SQL Server 2005 SP1 or later |
| **E\_EDM\_STANDARD\_APINOTSUPPORTED** | 0x800402F2 = The API is not supported in SOLIDWORKS PDM standard version |
| **E\_EDM\_STANDARD\_FEATURENOTSUPPORTED** | 0x800402ED = This feature is not supported in SOLIDWORKS PDM standard version |
| **E\_EDM\_STANDARD\_FEATURENOTSUPPORTED\_REFERLOG** | 0x800402F9 = This feature is not supported in SOLIDWORKS PDM standard version; refer to the log file for more information |
| **E\_EDM\_STANDARD\_PROFLOGINNOTSUPPORTED** | 0x800402F3 = Login not supported |
| **E\_EDM\_STANDARD\_SQLEDITIONMISMATCH** | 0x800402EC = Mismatch between SOLIDWORKS PDM standard version and Microsoft SQL |
| **E\_EDM\_STATE\_MULTIPLE\_BLOCKING\_WARNINGS\_FOUND** | 0x80040305 = Multiple blocking warnings found |
| **E\_EDM\_STATE\_MULTIPLE\_WARNINGS\_FOUND** | 0x80040304 = Multiple warnings found |
| **E\_EDM\_STATE\_NOT\_FOUND** | 0x80040216 = The specified state does not exist |
| **E\_EDM\_STATE\_REFERRING\_CRS\_CONDITION** | 0x80040303 = The workflow cannot be deleted since it is used in transition conditions |
| **E\_EDM\_SWDRW\_SETTO\_USE\_INDEPENDENT\_REV\_TABLE** | 0x800402FF = Independent type revision setting is used in the drawing |
| **E\_EDM\_SWFILE\_MISSING\_XMLSTREAM** | 0x800402F5 = SOLIDWORKS file missing XML stream |
| **E\_EDM\_SWSEC\_LICENSE\_CHECKIN\_FAILED** | 0x800402E7 = The check-in failed |
| **E\_EDM\_SWSEC\_LICENSE\_CHECKIN\_FAILED\_PRO** | 0x800402EF = Check-in failed in SOLIDWORKS PDM Professional |
| **E\_EDM\_SWSEC\_LICENSE\_CHECKIN\_FAILED\_STD** | 0x800402F1 = Check-in failed in SOLIDWORKS PDM standard version |
| **E\_EDM\_SWSEC\_LICENSE\_CHECKOUT\_FAILED** | 0x800402E6 = Check-out failed |
| **E\_EDM\_SWSEC\_LICENSE\_CHECKOUT\_FAILED\_PRO** | 0x800402EE = Check-out failed in SOLIDWORKS PDM Professional |
| **E\_EDM\_SWSEC\_LICENSE\_CHECKOUT\_FAILED\_STD** | 0x800402F0 = Check-out failed in SOLIDWORKS PDM standard version |
| **E\_EDM\_SWSEC\_LICENSE\_CONNECTION\_LOST** | 0x800402E9 = The connection was lost |
| **E\_EDM\_SWSEC\_LICENSE\_SERVERQUERY\_FAILED** | 0x800402E8 = The server query failed |
| **E\_EDM\_TEMPLATE\_IMPORT\_WITHOUT\_LOCAL\_VIEW** | 0x800402F6 = Template imported iwthout local view |
| **E\_EDM\_TOO\_MANY\_USERS** | 0x80040248 = The licensed maximum number of simultaneously logged-in users would be exceeded by this log-in; this log-in was refused |
| **E\_EDM\_TOOLBOX\_FILE\_LOCATED\_IN\_NONTOOLBOX\_FOLDER** | 0x800402FA = Toolbox file must be located in a Toolbox folder |
| **E\_EDM\_TRANSITION\_ACTION\_FAILED** | 0x80040234 = An error occurred when trying to execute a transition action |
| **E\_EDM\_UNC\_PATH\_ADDIN\_NOT\_SUPPORTED** | 0x800402DD =  Information cannot be retrieved from add-ins on a network drive; copy the file to the local hard disk and retry the operation |
| **E\_EDM\_UNSUPPORTED\_OS** | 0x800402D3 = The version of the operating system is not supported |
| **E\_EDM\_UNSUPPORTED\_PROGRAM\_VERSION** | 0x8004023E = The program requires a higher version of SOLIDWORKS PDM Professional than the installed version |
| **E\_EDM\_UNSUPPORTED\_SN\_TYPE** | 0x8004026F = The serial number type is not supported |
| **E\_EDM\_UPDATE\_ATT\_FAILED** | 0x8004020D = Could not update attributes during check in |
| **E\_EDM\_USER\_BLOCKED** | 0x80040265 = The administrator has blocked your login name in this file vault |
| **E\_EDM\_USER\_NAME\_ALREADY\_EXISTS** | 0x8004028A = The user name already exists |
| **E\_EDM\_USER\_NAME\_NOT\_UNIQUE** | 0x80040288 = The user name is not unique in the specified array of users |
| **E\_EDM\_USER\_NOT\_FOUND\_IN\_ARCHIVE\_SERVER** | 0x80040292 = The user name does not exist in the archive server |
| **E\_EDM\_VALUE\_NOT\_UNIQUE** | 0x8004022C = An attempt was made to save a duplicate value when a unique value is required |
| **E\_EDM\_VARIABLE\_NOT\_FOUND** | 0x80040252 = The specified card variable is missing |
| **E\_EDM\_VARIABLE\_USED\_IN\_COLUMN** | 0x80040244 = The variable cannot be deleted because it is used in a user-defined column |
| **E\_EDM\_VARIABLE\_USED\_IN\_EXPORT\_SCRIPT** | 0x800402AA = The variable cannot be deleted because it is used in a data export rule |
| **E\_EDM\_VARIABLE\_USED\_IN\_WORKFLOW\_STATE** | 0x800402EB = The variable cannot be deleted because it is used in a workflow state |
| **E\_EDM\_VAULT\_ALREADY\_EXISTS** | 0x8004024D = A vault with the same name already exists on the archive server |
| **E\_EDM\_VERSION\_MISMATCH** | 0x8004022E = The versions of the program and the file vault are incompatible |
| **E\_EDM\_WF\_HAS\_FILES** | 0x8004024A = The workflow contains files and cannot be deleted |
| **E\_EDM\_XREF\_OUTSIDE\_VAULT** | 0x8004026C = One or more of the file's referenced files are outside the file vault |
| **E\_ITEM\_CANNOT\_COPY\_ITEM** | 0x800402BA = You have selected items to copy; the items cannot be copied because they must be unique within the system |
| **E\_ITEM\_CYCLIC\_REFERENCE** | 0x800402CA =  Operation aborted because it would create a cyclic reference between items |
| **E\_ITEM\_ILLEGAL\_MOVE\_REFERENCED\_BY\_EXTERNAL** | 0x800402C8 = The object cannot be moved because the object or a sub-object is referenced by a locked item |
| **E\_ITEM\_ILLEGAL\_RENAME\_REFERENCED\_BY\_EXTERNAL** | 0x800402C9 = The object cannot be renamed because the object or a sub-object is referenced by a locked item |
| **E\_ITEM\_INVALID\_ITEM\_TYPE** | 0x800402BB = Invalid object type; only Item, ItemFolder, and files are supported by Item Explorer |
| **E\_ITEM\_INVALID\_LINK\_OPERATION** | 0x800402B8 = This operation cannot be performed on the selected items |
| **E\_ITEM\_INVALID\_LINK\_TYPE** | 0x800402B7 = Invalid link type; only two link types are supported by Item Explorer, static and auto-update |
| **E\_ITEM\_INVALID\_OBJECT** | 0x800402BD = Item object contains corrupted data |
| **E\_ITEM\_INVALID\_SOURCE** | 0x800402B5 = The selection contains items that are not valid for this operation |
| **E\_ITEM\_INVALID\_TARGET** | 0x800402B4 = The destination object is invalid for this operation |
| **E\_ITEM\_LINK\_DUPLICATED** | 0x800402B9 = The file is already added to this item |
| **E\_ITEM\_LOCKED\_ELSEWHERE** | 0x800402DF = Item is locked on another computer |
| **E\_ITEM\_MANY\_DYN\_LINKS** | 0x800402B6 = This item already has an auto-update link attached to it; items can have only one auto-update link at a time |
| **E\_ITEM\_NO\_ITEM\_GEN\_DEFINED** | 0x800402BC = No serial number generator has been set up to generate item numbers. Please do the following:   1. Launch SOLIDWORKS PDM Professional Administration Tool.- Create a serial number.- Open the Items administration node and select the serial number. |
| **E\_ITEM\_NOT\_CONNECTED** | 0x800402C1 = This item has no file linked or connected to it |
| **E\_ITEM\_NOT\_LOCKED** | 0x800402DE = Item has to be checked out to perform this operation |
| **E\_ITEM\_UP\_TO\_DATE** | 0x800402BE = The item is up to date |

# ![](dotnetimages/collapse.gif)Example

Client code can only access these return codes by handling the exception. For example, in C#:

> try
> {
>     // Some SOLIDWORKS PDM Professional call that results in an exception
> }
> catch (System.Runtime.InteropServices.ComException comEx)
> {
>     switch (comEx.ErrorCode)
>     {
>         case E\_EDM\_*xxx*:
>             // respond to *xxx*
>             break;
>         case E\_EDM\_*yyy*:
>             // respond to *yyy*
>             break;
>         default:
>             // Unexpected or cannot be handled silently
>             // Use IEdmVault5::GetErrorString or IEdmVault11::GetErrorMessage to prepare a message for the user or log
>             break;
>     }
> }

# ![](dotnetimages/collapse.gif)Remarks

HRESULT return codes are supported by the SOLIDWORKS PDM Professional API. You can pass the HRESULT code to the method [IEdmVault11::GetErrorMessage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorMessage.html) to get information about the code.

**NOTES:**

* Methods called from Visual Basic do not return the HRESULT code directly. Instead, the return codes are returned as an argument declared with the [retval] directive, if one exists. Visual Basic users can view the error codes returned by methods by implementing an error handler and checking the Number property of the Err object. The property is the HRESULT return code from the failing method.* The values shown in this topic are written in C++ style hexadecimal notation. In VB.NET, the value 0x80040200 is written as &H80040200.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.EPDMResultCode Namespace](EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode_namespace.html)

[IEdmVault5::GetErrorString Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetErrorString.html)

[IEdmVault11::GetErrorName Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorName.html)

[Return Codes](ReturnCodes.htm)