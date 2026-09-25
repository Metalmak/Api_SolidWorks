<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBatchGet Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBatchGet Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to get several files from the vault all at once.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBatchGet ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBatchGet ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBatchGet ``` | |

# ![](dotnetimages/collapse.gif)Example

[Batch Check Out Files (VB.NET)](Batch_Get_Files_Example_VBNET.htm)

[Batch Check Out Files (C#)](Batch_Get_Files_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).

To get several files at once:

1. Access this interface by calling [IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html), passing [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_BatchGet as a parameter.- Call [IEdmBatchGet::AddSelection](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~AddSelection.html) or [IEdmBatchGet::AddSelectionEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~AddSelectionEx.html) at least once.- Call [IEdmBatchGet::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~CreateTree.html) to compute the file reference tree and specify get and check-out options.- Optionally call [IEdmBatchGet::ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~ShowDlg.html) to display the Get or Check Out dialog box.- Call [IEdmBatchGet::GetFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~GetFiles.html) to get the files.

Using this interface is more efficient than calling [IEdmFile5::GetFileCopy](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFileCopy.html) and [IEdmFile5::LockFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockFile.html) for each file that you want to check out.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchGet Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)