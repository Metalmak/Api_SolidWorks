<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory2~Rollback.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback Method (IEdmHistory2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmHistory2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory2.html) : Rollback Method (IEdmHistory2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*historyItem*
:   [EdmHistoryItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html) to which to roll back

Rolls back the specified file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rollback( _    ByRef historyItem As EdmHistoryItem _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rollback(     ref EdmHistoryItem historyItem ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rollback(  &   EdmHistoryItem% historyItem ) ``` | |

#### Parameters

*historyItem*
:   [EdmHistoryItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html) to which to roll back

# ![](dotnetimages/collapse.gif)Example

See the [IEdmHistory3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

To populate historyItem, get the collection of history items by calling [IEdmHistory::GetHistory](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~GetHistory.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistory2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory2.html)

[IEdmHistory2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017