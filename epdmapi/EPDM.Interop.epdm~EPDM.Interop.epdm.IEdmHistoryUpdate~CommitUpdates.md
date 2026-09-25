<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate~CommitUpdates.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CommitUpdates Method (IEdmHistoryUpdate) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmHistoryUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate.html) : CommitUpdates Method (IEdmHistoryUpdate) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Commits all of the updates in this batch.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CommitUpdates() ``` | |

| C# |  |
| --- | --- |
| ``` void CommitUpdates() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CommitUpdates(); ``` | |

# ![](dotnetimages/collapse.gif)Example

See the [IEdmHistoryUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method must be called after calling [IEdmHistoryUpdate::UpdateVersionComment](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate~UpdateVersionComment.html) and [IEdmHistoryUpdate::UpdateRevisionComment](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate~UpdateRevisionComment.html), or all updates are discarded.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistoryUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate.html)

[IEdmHistoryUpdate Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008