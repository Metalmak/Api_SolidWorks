<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBatchUpdate2 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBatchUpdate2 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to set the values of several file and folder card variables all at once.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBatchUpdate2 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBatchUpdate2 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBatchUpdate2 ``` | |

# ![](dotnetimages/collapse.gif)Example

[Batch Update Card Variables (VB.NET)](Batch_Update_Variables_Example_VBNET.htm)

[Batch Update Card Variables (C#)](Batch_Update_Variables_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* supersedes IEdmBatchUpdate, which can only update file variables.

To set the values of file and folder card variables:

1. Access this interface by calling [IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html), passing in [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_BatchUpdate.- Call [IEdmBatchUpdate2::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~SetVar.html) once for each file card variable you want to update. You must first check out the files whose card varibles you want to update.- Call [IEdmBatchUpdate2::SetFolderVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~SetFolderVar.html) once for each folder card variable you want to update.- Call [IEdmBatchUpdate2::CommitUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~CommitUpdate.html) to commit all of the file and folder card variable changes.

Prior to SOLIDWORKS PDM Professional 6.2, the only way to set file card variables was to use [IEdmEnumeratorVariable](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable9.html), which can handle only one file or folder card variable at a time.  As of SOLIDWORKS PDM Professional 6.2, you should use IEdmBatchUpdate2, which can handle several file and folder card variables at a time.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUpdate2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)