<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3~GetSortedHistory.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetSortedHistory Method (IEdmHistory3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmHistory3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3.html) : GetSortedHistory Method (IEdmHistory3) |

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

Gets the history listing for the specified history types.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetSortedHistory( _    ByRef ppoRetHistory() As EdmHistoryItem, _    Optional ByVal lEdmHistoryTypes As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSortedHistory(     out EdmHistoryItem[] ppoRetHistory,    System.int lEdmHistoryTypes ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSortedHistory(  &   [Out] array<EdmHistoryItem>^ ppoRetHistory, &   System.int lEdmHistoryTypes ) ``` | |

#### Parameters

*ppoRetHistory*
:   Array of [EdmHistoryItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html) structures; one structure for each history item (see **Remarks**)

*lEdmHistoryTypes*
:   Combination of [EdmHistoryType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html) bits; indicates the kinds of records to retrieve

# ![](dotnetimages/collapse.gif)Example

See the [IEdmHistory3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method works in both Web 2 and thick client applications.

Call this method after calling [IEdmHistory::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~AddFile.html) and [IEdmHistory::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~AddFolder.html).

The returned array of history items in ppoRetHistory is sorted with the most recent records at the beginning.

Call [IEdmHistory3::GetEventDescription](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3~GetEventDescription.html), passing one of the EdmHistoryItem structures returned by this method, to obtain its event description.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistory3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3.html)

[IEdmHistory3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3_members.html)

[IEdmHistory2::Rollback Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory2~Rollback.html)

[IEdmHistory::GetHistory Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~GetHistory.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2020