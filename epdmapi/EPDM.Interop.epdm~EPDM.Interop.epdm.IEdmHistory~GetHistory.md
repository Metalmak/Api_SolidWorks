<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~GetHistory.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetHistory Method (IEdmHistory) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmHistory Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html) : GetHistory Method (IEdmHistory) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetHistory*
:   Array of [EdmHistoryItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html) structures; one structure for each history item (see **Remarks**)

*lEdmHistoryTypes*
:   Combination of [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html) bits; indicates the kinds of records to retrieve

Gets the unsorted history listing for the specified history types.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetHistory( _    ByRef ppoRetHistory() As EdmHistoryItem, _    Optional ByVal lEdmHistoryTypes As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetHistory(     out EdmHistoryItem[] ppoRetHistory,    System.int lEdmHistoryTypes ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetHistory(  &   [Out] array<EdmHistoryItem>^ ppoRetHistory, &   System.int lEdmHistoryTypes ) ``` | |

#### Parameters

*ppoRetHistory*
:   Array of [EdmHistoryItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html) structures; one structure for each history item (see **Remarks**)

*lEdmHistoryTypes*
:   Combination of [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html) bits; indicates the kinds of records to retrieve

# ![](dotnetimages/collapse.gif)Remarks

Call this method after calling [IEdmHistory::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~AddFile.html) and [IEdmHistory::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~AddFolder.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistory Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html)

[IEdmHistory Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory_members.html)

[IEdmHistory2::Rollback Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory2~Rollback.html)

[IEdmHistory3::GetSortedHistory Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3~GetSortedHistory.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4