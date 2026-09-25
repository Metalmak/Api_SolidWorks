<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBatchDelete3 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBatchDelete3 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to delete several files and folders from the vault all at once.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBatchDelete3     Inherits IEdmBatchDelete, IEdmBatchDelete2  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBatchDelete3 : IEdmBatchDelete, IEdmBatchDelete2  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBatchDelete3 : public IEdmBatchDelete, IEdmBatchDelete2  ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This interface extends [IEdmBatchDelete2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete2.html) by adding [IEdmBatchDelete3::GetCommitErrors](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3~GetCommitErrors.html) which shows the errors that occurred during [IEdmBatchDelete::CommitDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~CommitDelete.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchDelete3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)