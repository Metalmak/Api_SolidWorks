<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html -->

![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/drpdown.gif)
![](dotnetimages/drpdown_orange.gif)
![](dotnetimages/copycode.gif)
![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |

| EdmCmdData Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCmdData Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains command data.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmCmdData     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmCmdData : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmCmdData : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmCmdData{
   integer [mlObjectID1](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mlObjectID1.html);
   integer [mlObjectID2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mlObjectID2.html);
   integer [mlObjectID3](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mlObjectID3.html);
   integer [mlObjectID4](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mlObjectID4.html);
   string [mbsStrData1](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mbsStrData1.html);
   string [mbsStrData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mbsStrData2.html);
   string [mbsStrData3](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mbsStrData3.html);
   integer [mlLongData1](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mlLongData1.html);
   integer [mlLongData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mlLongData2.html);
   integer [mlLongData3](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mlLongData3.html);
   object\* [mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData~mpoExtra.html);
};

# ![](dotnetimages/collapse.gif)Example

[Notify User When File Changes State (VB.NET)](Notify_User_When_File_Changes_State_Example_VBNET.htm)

[Notify User When File Changes State (C#)](Notify_User_When_File_Changes_State_Example_CSharp.htm)

[Change Card Variables Add-in (VB.NET)](Change_Card_Variables_Addin_Example_VBNET.htm)

[Change Card Variables Add-in (C#)](Change_Card_Variables_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

SOLIDWORKS PDM Professional passes an array of 0 or more EdmCmdData structures when it calls to [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html).

Typically there is one structure for each file affected by the command. For instance, if the user has selected five files and two folders and launches an add-in-implemented menu command, the add-in receives seven structures, one for each of the selected files and folders. If the reason for calling IEdmAddIn5::OnCmd is a hook on a command like Check out, Check in, Get, Change state, etc., the add-in receives one structure per file. The actual meaning of each structure member varies with the reason for calling IEdmAddIn5::OnCmd. The reason for a call can be determined by examining the meCmdType member of the [EdmCmd structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html) that is passed in the first argument of IEdmAddIn5::OnCmd.

The following tables contain all members for each [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html). Members that are not listed for a certain type of command do not use EdmCmdData.

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_ActivateAPITab

When a custom vault view tab is selected in a vault view in File Explorer, sends only to the add-in that adds the custom vault view tab to File Explorer.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mbsStrData3 | string | Unique ID of this control |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreExploreInit

When a new instance of File Explorer to about to be created, this event is sent to allow you to create custom tabs in the vault view in File Explorer. This event does not provide any EdmCmdData information. But you will receive a pointer to the IEdmCmdMgr6 interface in the [EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) member. In the event handler, call [IEdmCmdMgr6::AddValtViewTab](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr6~AddVaultViewTab.html) for each tab you want to add to the vault view in File Explorer.

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_Menu

The user has activated a menu item or toolbar button that your add-in has added. This command returns a combination of refresh flags in the mlEdmRefreshFlags member of the [EdmCmd structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html).

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file; 0 if a folder is selected |
| mlObjectID2 | integer | ID of folder; 0 if a file is selected |
| mlObjectID3 | integer | ID of parent folder of the selected file or folder |
| mbsStrData1 | string | Name of file or folder, not the full path |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_CardButton

The user clicked a button in a file or folder data card, and the button is connected to an add-in. This notification is also sent when the user clicks **OK** or **Apply** in the card.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file for which the card is displayed; 0 for folder cards |
| mlObjectID2 | integer | ID of folder; parent folder ID for file data cards |
| mlObjectID3 | integer | ID of file data card |
| mbsStrData1 | string | Name of active configuration; can be changed to switch to a new configuration |
| mbsStrData2 | string | Path to file |
| mlLongData1 | integer | Optionally return a [EdmCardFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardFlag.html) return code here |
| mlLongData2 | integer | Optionally return the ID of a card control to set focus to here |
| mpoExtra | object\* | Pointer to an [IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html) interface with the names of all configurations |

Note: You will also receive pointers to the [IEdmEnumeratorVariable5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html) and [IEdmCard5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html) interfaces in the [EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) member. The content of the [EdmCmd::mbsComment](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbsComment.html) member is the button command string entered in the Card Editor.

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_CardInput

The user has modified some data in a file or folder data card.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of the modified card control |
| mlObjectID2 | integer | ID of the file; 0 for folder cards |
| mlObjectID3 | integer | ID of the folder |
| mlObjectID4 | integer | ID of the card |
| mbsStrData1 | string | Name of the active configuration |
| mbsStrData2 | string | Full path to the file |
| mlLongData1 | integer | ID of the updated variable |
| mpoExtra | object\* | Pointer to an [IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html) interface with all configuration names |

Note: You will also receive pointers to the [IEdmEnumeratorVariable5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html) and [IEdmCard5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html) interfaces in the [EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) member. The content of the [EdmCmd::mbsComment](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbsComment.html) member is the name of the modified variable.

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_CardListSrc

A file or folder data card containing a list box or combo box is displayed. The add-in’s [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) method is given the opportunity to fill in the rows in the list instead of using the list contents defined in the card editor.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of the card control |
| mlObjectID2 | integer | ID of the file; 0 for folder cards |
| mlObjectID3 | integer | ID of the folder |
| mlObjectID4 | integer | ID of the card |
| mbsStrData1 | string | Name of the active configuration |
| mbsStrData2 | string | Full path to the file |
| mbsStrData3 | string | Name of the control’s variable |
| mlLongData1 | integer | ID of the control’s variable |
| mpoExtra | object\* | Pointer to an [IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html) interface with all configuration names |

Note: You will also receive a pointer to the [IEdmEnumeratorVariable5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html) and [IEdmCard5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html) interfaces via the [EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) member. The content of the [EdmCmd::mbsComment](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbsComment.html) member is the return value from your add-in's IEdmAddIn5::OnCmd implementation. This variable should be set to a newline delimited list of strings to be inserted into the list box or combo box. Leave this variable untouched to use the standard values from the card editor.

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_DeSelectItem

When an item is deselected in a vault view in File Explorer, sends only to the add-in that adds a vault view tab to File Explorer.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mbsStrData1 | string | File name |
| mbsStrData2 | string | Folder name |
| mbsStrData3 | string | Unique ID of this control |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreAdd

A file is about to be added.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of parent folder |
| mbsStrData1 | string | Local file path |
| mlLongData1 | integer | 0 for normal files; 1 for network sharing links |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostAdd

A file has been added.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of parent folder |
| mlObjectID2 | integer | ID of file |
| mbsStrData1 | string | Full path to file |
| mlLongData1 | integer | 0 for normal files; 1 for network sharing links |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreAddFolder

A folder is about to be added.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID3 | integer | ID of parent folder |
| mbsStrData1 | string | Path to new folder |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostAddFolder

A folder has been added.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of new folder |
| mlObjectID3 | integer | ID of parent folder |
| mbsStrData1 | string | Path to the new folder |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreCopy and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostCopy

A file is copied.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of destination folder |
| mlObjectID2 | integer | ID of file |
| mlObjectID3 | integer | ID of source folder |
| mbsStrData1 | string | Source file path |
| mbsStrData2 | string | Destination file path |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreCopyFolder

A folder is about to be copied.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID2 | integer | Source folder ID |
| mlObjectID3 | integer | Destination parent folder ID |
| mbsStrData1 | string | Path of new folder |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostCopyFolder

A folder has been copied.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of new folder |
| mlObjectID2 | integer | Source folder ID |
| mlObjectID3 | integer | Destination parent folder ID |
| mbsStrData1 | string | Path of new folder |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreDelete

A file is about to be deleted.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to delete |
| mlObjectID2 | integer | ID of folder to delete file in |
| mbsStrData1 | string | Path to file to delete |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostDelete

A file has been deleted.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file that was deleted |
| mlObjectID2 | integer | ID of folder in which the file was deleted |
| mbsStrData1 | string | Path to file that was deleted |
| mlLongData1 | integer | Number of folders to which the file is shared |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreDeleteFolder and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostDeleteFolder

A folder is deleted.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of folder to delete |
| mbsStrData1 | string | Path to folder to delete |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreGet and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostGet

A file is retrieved from the archive to the local hard disk.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to get |
| mlObjectID2 | integer | ID of folder to get file to; 0 to retrieve a file to a temporary folder |
| mbsStrData1 | string | Destination file path |
| mlLongData1 | integer | Version number of file to get |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreLabel and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostLabel

A label is being created on files and/or folders.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to set label on; 0 for folders |
| mlObjectID2 | integer | ID of folder to set label on; parent folder ID for files; note that this ID is zero when creating a file label via the API, since that does not happen within the context of a folder |
| mlObjectID3 | integer | 0 for EdmCmd\_PreLabel; ID of the created label for EdmCmd\_PostLabel |
| mbsStrData1 | string | Label |
| mbsStrData2 | string | Path to file or folder to create label for; note that this member will only contain the file name without path when file labels are created via the API, since that is not done within the context of a folder |
| mlLongData1 | integer | Non 0 if label is created recursively for this folder, 0 otherwise |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreLabelDelete, [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostLabelDelete, [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreLabelModify, and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostLabelModify

A label is being deleted or modified.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of the label |
| mbsStrData1 | string | Label |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreLabelAddItem and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostLabelAddItem

A file or folder is being added to an existing label.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID the label |
| mlObjectID2 | integer | ID of the file to add; 0 for folders |
| mlObjectID3 | integer | ID of the folder to add; 0 for files |
| mbsStrData1 | string | Label |
| mlLongData1 | integer | Non 0 if a folder is added recursively, 0 otherwise |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreLock and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostLock

A file is checked out.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to check out |
| mlObjectID2 | integer | ID of folder where put checked-out file |
| mbsStrData1 | string | Path to file |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreMove and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostMove

A file is moved from one folder to another one.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to move |
| mlObjectID2 | integer | ID of source folder |
| mlObjectID3 | integer | ID of destination folder |
| mbsStrData1 | string | Source file path |
| mbsStrData2 | string | Destination file path |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreMoveFolder and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostMoveFolder

A folder is moved from one parent folder to another one.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of folder to move |
| mlObjectID2 | integer | ID of source parent folder |
| mlObjectID3 | integer | ID of destination parent folder |
| mbsStrData1 | string | Source folder path |
| mbsStrData2 | string | Destination folder path |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreRename and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostRename

A file is renamed.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to rename |
| mlObjectID2 | integer | ID of the file's parent folder |
| mbsStrData1 | string | Old file name |
| mbsStrData2 | string | New file name |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreRenameFolder and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostRenameFolder

A folder is renamed.

|  |  |  |
| --- | --- | --- |
| **EdCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of folder to rename |
| mlObjectID2 | integer | ID of the folder's parent folder |
| mbsStrData1 | string | Old folder name |
| mbsStrData2 | string | New folder name |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreShare and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostShare

A file is shared from one folder to another one.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to share |
| mlObjectID2 | integer | ID of folder to share file from |
| mlObjectID3 | integer | ID of folder to share file to |
| mbsStrData1 | string | Source file path |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreState and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostState

The user changes the workflow state of a file.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to change state on |
| mlObjectID2 | integer | ID of the file's parent folder |
| mlObjectID3 | integer | ID of the transition (state change) to perform |
| mlObjectID4 | integer | ID of user that performs the state change |
| mbsStrData1 | string | Path to file |
| mbsStrData2 | string | Name of the destination state |
| mlLongData1 | integer | Source state ID |
| mlLongData2 | integer | Destination state ID |

You will receive an [IEdmCmdNode](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdNode.html) interface in the mpoExtra member of the struct as of version 2011 during the change state operation.

#### CmdType.EdmCmd\_PreUndoLock and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostUndoLock

The user runs the command Undo check-out on a file. (This is the same as check-in of an unmodified file.)

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to perform undo check-out on |
| mlObjectID2 | integer | ID of the file's parent folder |
| mbsStrData1 | string | Path to file |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreUnlock and [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PostUnlock

The user runs a check-in on a modified file. (Checking in unmodified files results in an Undo check-out operation.)

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to check in |
| mlObjectID2 | integer | ID of the file's parent folder |
| mbsStrData1 | string | Path to the file |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_SelectItem

When an item is selected in a vault view in File Explorer, sends only to the add-in that adds a vault view tab to File Explorer.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of the item |
| mbsStrData1 | string | File name |
| mbsStrData2 | string | Folder name |
| mbsStrData3 | string | Unique ID of this control |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_SerialNo

New serial number(s) should be generated by your add-in.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of file to generate serial number for; 0 if not generated for a file |
| mlObjectID2 | integer | ID of the file's parent folder |
| mlObjectID3 | integer | ID of the file data card |
| mlObjectID4 | integer | ID of the control in the file data card |
| mbsStrData1 | string | Return the generated serial number here (C++ users must allocate the string with the Win32 function **SysAllocString**) |
| mbsStrData2 | string | Path to file; folder path if the serial number is created for the template manager as part of the folder name |
| mbsStrData3 | string | Name of configuration |
| mlLongData1 | integer | Serial number counter value |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskSetup

This call is made to your add-in when the [task](Tasks.htm) definition property dialog box is called. The call makes it possible for you to add your own custom pages to the wizard. The [EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) pointer points to [IEdmTaskProperties](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html), the interface of the task definition.

You typically do the following in this call:

* Call [IEdmTaskProperties::SetSetupPages](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetSetupPages.html) to add property dialog box pages.* Call [IEdmTaskProperties::SetMenuCmds](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetMenuCmds.html) to add menu commands to show in File Explorer.* Update the [IEdmTaskProperties::TaskFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~TaskFlags.html) property to inform the framework about what your add-in is capable of.

None of the members in the EdmCmdData structure are used.

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskSetupButton

This call is made to your add-in when the [task](Tasks.htm) definition property dialog box is closed. The [EdmCmd::mbsComment](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbsComment.html) string is either "OK" or "Cancel", depending on how the dialog box closed. (The string is the same in all localized versions of the program.) The call makes it possible for you to save your own properties when **OK** is clicked. You can prevent the dialog box from closing by setting the [EdmCmd::mbCancel](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbCancel.html) member to true. You can return the name of an add-in page to set focus to in the [EdmCmd::mbsComment](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbsComment.html) string if [EdmCmd::mbCancel](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbCancel.html) is set to true. [EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) points to [IEdmTaskProperties](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html), the interface of the task definition.

None of the members in the EdmCmdData structure are used.

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskDetails

This call is made to your add-in when the [task](Tasks.htm) details dialog box is displayed from the task list in the administration tool. You must specify the flag [EdmTaskFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskFlag.html).EdmTask\_SupportsDetails in the [IEdmTaskProperties::TaskFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~TaskFlags.html) property in order to get the EdmCmd\_TaskDetails call. You can set the flag when you get the [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskSetup call. [EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) points to [IEdmTaskInstance](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html), the interface of the task instance.

The EdmCmd::mpoExtra pointer should be set to your implementation of the extra page. The framework keeps this pointer referenced until the dialog box is closed. You return the window handle of the extra page in the member [EdmCmd::mlParentWnd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mlParentWnd.html). The property dialog box calls ShowWindow when the page is displayed or hidden.

None of the members in the EdmCmdData structure are used.

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskRun

This is the callback that is called when the actual work of the [task](Tasks.htm) is supposed to be executed. The task is usually executed on a remote server so you must not display any user interface during this call. See the OnTaskRun function in the [task sample code](TaskSample.htm) for an example of how to return status information and errors to the user.

The [EdmCmd::mlCurrentFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mlCurrentFolderID.html) argument is the ID of the current folder when the task was launched. It is zero if the task was launched from the administration tool.

[EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) points to the [IEdmTaskInstance](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html) interface of the task instance.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of the selected object ([IEdmObject5::ID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5~ID.html)) |
| mlObjectID2 | integer | Parent folder ID if the selected object is a file |
| mbsStrData1 | string | Complete file system path to the object |
| mbsStrData2 | string | Configuration name if the object is a file |
| mlLongData1 | integer | [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) constant telling what kind of object this is |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskLaunch

You need to specify the EdmTask\_SupportsInitExec in the [IEdmTaskProperties::TaskFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~TaskFlags.html) property in order to get this call. The launch call makes it possible for you to display a user interface where the user selects files or enters data in a custom dialog box. As an alternative, you can create a card with the card editor and use that instead. [EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) points to [IEdmTaskInstance](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html), the interface of the task instance in this call.

You can return a dialog box implementation (user control) in the EdmCmd::mpoExtra argument. In this case you must also return the window of the control in [EdmCmd::mlParentWnd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mlParentWnd.html). The form is then put in the same parent dialog box as the card, if you are using one.

You can set [EdmCmd::mbCancel](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbCancel.html) to true to halt further execution of the task.

The call can update the selection of objects to execute the task on by altering the content of the EdmCmdData structure.

|  |  |  |
| --- | --- | --- |
| **EdmCmdData Members** | **Type** | **Description** |
| mlObjectID1 | integer | ID of the selected object ([IEdmObject5::ID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5~ID.html)) |
| mlObjectID2 | integer | Parent folder ID if the selected object is a file |
| mbsStrData1 | string | Complete file system path to the object |
| mbsStrData2 | string | Configuration name if the object is a file |
| mlLongData1 | integer | [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) constant telling what kind of object this is |
| mlLongData2 | integer | Local version number of the file |

#### [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskLaunchButton

This callback is made if the framework displays its own dialog box during the launching of a task. The framework displays its own dialog box if a card has been selected for the task or if you returned a user control from the [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskLaunch hook. [EdmCmd::mbsComment](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbsComment.html) contains the string "OK" or "Cancel", depending on which button was clicked. The strings are the same on all localized versions of the program. [EdmCmd::mpoExtra](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mpoExtra.html) points to IEdmTaskInstance, the interface of the task. You can set [EdmCmd::mbCancel](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mbCancel.html) to true to halt further execution of the task.

None of the members in the EdmCmdData structure are used.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmCmdData Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010