<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmCallback Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmCallback Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Monitors the progress of a supported API operation.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmCallback ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmCallback ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmCallback ``` | |

# ![](dotnetimages/collapse.gif)Example

[Create Card View (VB.NET)](Create_Card_View_Example_VBNET.htm)

[Create Card View (C#)](Create_Card_View_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).

This callback interface works only with API methods that provide a poCallback argument. For example:

* [IEdmFolder5::CreateCardView](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateCardView.html)* [IEdmBatchAdd::CommitAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~CommitAdd.html)* [IEdmBatchChangeState::ChangeState](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~ChangeState.html)* [IEdmBatchDelete::CommitDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~CommitDelete.html)* [IEdmBatchUpdate2::CommitUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~CommitUpdate.html)* [IEdmClearLocalCache::CommitClear](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache~CommitClear.html)* [IEdmUserMgr8::CreateUserPicture](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8~CreateUserPicture.html)* [IEdmVault10::CreateCardViewEx2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10~CreateCardViewEx2.html)* [IEdmVault11::CreateNewVault](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~CreateNewVault.html)

To use this interface:

1. Create a new class.- Implement all of the methods of IEdmCallback in the new class.- Call one of the API methods whose progress you want to monitor, setting its poCallback argument to a pointer to the new class.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmFolder5::CreateCardView Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateCardView.html)

[IEdmEnumeratorVariable5::StoreValuesFromDatabase Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~StoreValuesFromDatabase.html)