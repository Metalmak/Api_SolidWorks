<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmHistoryUpdate Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmHistoryUpdate Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access the version and revision comments of files.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmHistoryUpdate ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmHistoryUpdate ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmHistoryUpdate ``` | |

# ![](dotnetimages/collapse.gif)Example

[Get Histories of Files (VB.NET)](Get_Histories_of_Files_Example_VBNET.htm)

[Get Histories of Files (C#)](Get_Histories_of_Files_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).

To use this interface:

1. Access this interface by calling IEdmVault7::CreateUtility with eType set to [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_HistoryUpdate.- Call [IEdmHistoryUpdate::UpdateRevisionComment](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate~UpdateRevisionComment.html) one or more times to add revision comments to the batch.- Call [IEdmHistoryUpdate::UpdateVersionComment](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate~UpdateVersionComment.html) one or more times to add version comments to the batch.- Call [IEdmHistoryUpdate::CommitUpdates](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate~CommitUpdates.html) to commit the batch of changes to the database.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistoryUpdate Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)