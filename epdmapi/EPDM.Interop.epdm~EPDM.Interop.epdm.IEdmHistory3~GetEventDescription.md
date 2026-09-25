<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3~GetEventDescription.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetEventDescription Method (IEdmHistory3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmHistory3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3.html) : GetEventDescription Method (IEdmHistory3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*historyItem*
:   [EdmHistoryItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html) (see **Remarks**)

*eLancode*
:   Localization language as defined in [EdmLangCode](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLangCode.html)

Gets the event description for the specified history item in the specified language.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetEventDescription( _    ByRef historyItem As EdmHistoryItem, _    Optional ByVal eLancode As EdmLangCode _ ) As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetEventDescription(     ref EdmHistoryItem historyItem,    EdmLangCode eLancode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetEventDescription(  &   EdmHistoryItem% historyItem, &   EdmLangCode eLancode ) ``` | |

#### Parameters

*historyItem*
:   [EdmHistoryItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryItem.html) (see **Remarks**)

*eLancode*
:   Localization language as defined in [EdmLangCode](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLangCode.html)

#### Return Value

History item event description

# ![](dotnetimages/collapse.gif)Example

See the [IEdmHistory3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IEdmHistory3::GetSortedHistory](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3~GetSortedHistory.html) to specify a historyItem.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistory3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3.html)

[IEdmHistory3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2020