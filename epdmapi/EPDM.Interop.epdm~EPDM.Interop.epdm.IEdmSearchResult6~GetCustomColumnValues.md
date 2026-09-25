<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~GetCustomColumnValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCustomColumnValues Method (IEdmSearchResult6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearchResult6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6.html) : GetCustomColumnValues Method (IEdmSearchResult6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetColValues*
:   Array of string values (see **Remarks**)

Gets the custom column values returned in this favorite search result.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetCustomColumnValues( _    ByRef ppoRetColValues() As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetCustomColumnValues(     out System.string[] ppoRetColValues ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetCustomColumnValues(  &   [Out] System.array<String^>^ ppoRetColValues ) ``` | |

#### Parameters

*ppoRetColValues*
:   Array of string values (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSearch10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

ppoRetColValues is not null only for favorite search results that show custom columns.

If the favorite search result:

* Does not have custom columns,

* [ISearch10::GetFirstFavoriteResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10~GetFirstFavoriteResult.html) is called with bGetCustomColumns set to false, or

* [IEdmSearch5::GetFirstResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~GetFirstResult.html) is called,

then ppoRetColValues is null.

The ppoRetColValues array elements map to the fields in the [EdmListCol](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol.html) structures in the array (ppoRetColsInfo) that is returned by [IEdmSearchResult6::GetCustomColumnsInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~GetCustomColumnsInfo.html) as follows:

size\_of\_ppoRetColValues = (size\_of\_ppoRetColsInfo) \* (6 EdmListCol fields)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearchResult6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6.html)

[IEdmSearchResult6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021