<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBatchChangeState5 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState5_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBatchChangeState5 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to change states or revoke transitions of several files all at once.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBatchChangeState5     Inherits IEdmBatchChangeState, IEdmBatchChangeState2, IEdmBatchChangeState3, IEdmBatchChangeState4  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBatchChangeState5 : IEdmBatchChangeState, IEdmBatchChangeState2, IEdmBatchChangeState3, IEdmBatchChangeState4  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBatchChangeState5 : public IEdmBatchChangeState, IEdmBatchChangeState2, IEdmBatchChangeState3, IEdmBatchChangeState4  ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This interface extends [IEdmBatchChangeState4](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4.html) by allowing users to include parent files in the [file reference tree to revoke transactions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2~CreateTreeForRevoke.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchChangeState5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState5_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)