<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~GetCustomColumnsInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCustomColumnsInfo Method (IEdmSearchResult6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearchResult6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6.html) : GetCustomColumnsInfo Method (IEdmSearchResult6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetColsInfo*
:   Array of [EdmListCol](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol.html) structures (see **Remarks**)

Gets the custom column headers for this favorite search result.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetCustomColumnsInfo( _    ByRef ppoRetColsInfo() As EdmListCol _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetCustomColumnsInfo(     out EdmListCol[] ppoRetColsInfo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetCustomColumnsInfo(  &   [Out] array<EdmListCol>^ ppoRetColsInfo ) ``` | |

#### Parameters

*ppoRetColsInfo*
:   Array of [EdmListCol](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol.html) structures (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSearch10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

ppoRetColsInfo is not null only for favorite search results that show custom columns.

If the favorite search result:

* Does not have custom columns,

* [ISearch10::GetFirstFavoriteResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10~GetFirstFavoriteResult.html) is called with bGetCustomColumns set to false, or

* [IEdmSearch5::GetFirstResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~GetFirstResult.html) is called,

then ppoRetColsInfo is null.

The six fields in each structure returned in the ppoRetColsInfo array map to the elements in the array (ppoRetColValues) returned by [IEdmSearchResult6::GetCustomColumnValues](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~GetCustomColumnValues.html) as follows:

size\_of\_ppoRetColValues = (size\_of\_ppoRetColsInfo) \* (6 EdmListCol fields)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearchResult6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6.html)

[IEdmSearchResult6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021