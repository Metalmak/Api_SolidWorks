<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBatchDelete Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBatchDelete Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to delete several files and folders from the vault at once.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBatchDelete ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBatchDelete ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBatchDelete ``` | |

# ![](dotnetimages/collapse.gif)Example

[Batch Delete Files and Folders from Vault (VB.NET)](Batch_Delete_Files_and_Folders_Example_VBNET.htm)

[Batch Delete Files and Folders from Vault (C#)](Batch_Delete_Files_and_Folders_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* is extended by [IEdmBatchDelete2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete2.html).

To delete several files and folders from the vault at once:

1. Access this interface by calling [IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html), passing [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_BatchDelete as a parameter.- Call [IEdmBatchDelete::AddFileByID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFileByID.html), [IEdmBatchDelete::AddFileByPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFileByPath.html), or [IEdmBatchDelete::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFolder.html) one or more times to add files and folders to the batch for deletion.- Call [IEdmBatchDelete::ComputePermissions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~ComputePermissions.html) to prepare the delete operation.- Optionally call [IEdmBatchDelete2::ShowWarningDlg2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete2~ShowWarningDlg2.html) to display a message about any errors found in step 3.- Call [IEdmBatchDelete::CommitDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~CommitDelete.html) to delete the files and folders added to the batch.- Optionally call [IEdmBatchDelete::ShowCommitErrorsDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~ShowCommitErrorsDlg.html) or [IEdmBatchDelete3::GetCommitErrors](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3~GetCommitErrors.html) to get any errors that might have occurred in step 5.

Using IEdmBatchDelete is more efficient than calling [IEdmFolder5::DeleteFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFile.html) or [IEdmFolder5::DeleteFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFolder.html) multiple times.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchDelete Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)