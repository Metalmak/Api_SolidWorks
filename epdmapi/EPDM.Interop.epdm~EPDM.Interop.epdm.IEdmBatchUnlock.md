<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBatchUnlock Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBatchUnlock Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to unlock, check in, or undo check-outs of multiple files all at once.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBatchUnlock ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBatchUnlock ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBatchUnlock ``` | |

# ![](dotnetimages/collapse.gif)Example

[Batch Check In Files (C#)](Batch_Unlock_Files_Example_CSharp.htm)

[Batch Check In Files (VB.NET)](Batch_Unlock_Files_Example_VBNET.htm)

[Access Check-in Flags in Check out Dialog (C#)](Access_Check-in_Flags_in_Check_in_Dialog_Example_CSharp.htm)

[Access Check-in Flags in Check out Dialog (VB.NET)](Access_Check-in_Flags_in_Check_in_Dialog_Example_VBNET.htm)

[Prevent Admin from Checking In File (C#)](Prevent_Admin_from_Checking_In_File_Example_CSharp.htm)

[Prevent Admin from Checking In File (VB.NET)](Prevent_Admin_from_Checking_In_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* is extended by [IEdmBatchUnlock2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock2.html).

To unlock, check in, or undo the check-outs of multiple files in one batch:

1. Access this interface by calling [IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html), passing in [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_BatchUnlock.- Call [IEdmBatchUnlock::AddSelection](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~AddSelection.html) to specify the files to unlock.- Call [IEdmBatchUnlock::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~CreateTree.html) to create the file reference tree.- Optionally call [IEdmBatchUnlock::ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~ShowDlg.html) to display the SOLIDWORKS PDM Professional Check In or Undo Check Out dialog box.- Call [IEdmBatchUnlock::GetFileList](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~GetFileList.html) to get the files affected by the unlock operation.- Call [IEdmBatchUnlock::UnlockFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~UnlockFiles.html) to perform the batch unlock operation.

Using this interface to unlock, check in, or undo check-outs is more efficient than calling [IEdmFile5::UnlockFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UnlockFile.html) or [IEdmFile5::UndoLockFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UndoLockFile.html) for each file.

You can obtain an [IEdmRefItemContainer](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItemContainer.html) interface from IEdmBatchUnlock by assignment (QueryInterface in C++).

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUnlock Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)