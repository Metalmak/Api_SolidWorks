<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10~GetFirstFavoriteResult.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstFavoriteResult Method (IEdmSearch10) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10.html) : GetFirstFavoriteResult Method (IEdmSearch10) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsFavName*
:   Name of a favorite search

*bGetCustomColumns*
:   True to retrieve custom column information, false to not

Gets the first file or folder that matches the favorite search criteria.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstFavoriteResult( _    ByVal bsFavName As System.String, _    Optional ByVal bGetCustomColumns As System.Boolean _ ) As IEdmSearchResult5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmSearchResult5 GetFirstFavoriteResult(     System.string bsFavName,    System.bool bGetCustomColumns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmSearchResult5^ GetFirstFavoriteResult(  &   System.String^ bsFavName, &   System.bool bGetCustomColumns ) ``` | |

#### Parameters

*bsFavName*
:   Name of a favorite search

*bGetCustomColumns*
:   True to retrieve custom column information, false to not

#### Return Value

[IEdmSearchResult5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult5.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSearch10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

If bGetCustomColumns is set to true and custom columns exist in the search results of bsFavName, then use [IEdmSearchResult6::GetCustomColumnsInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~GetCustomColumnsInfo.html) and [IEdmSearchResult6::GetCustomColumnValues](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~GetCustomColumnValues.html) to see the custom column information.

After calling this method, call [IEdmSearch5::GetNextResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~GetNextResult.html) repeatedly to retrieve the rest of the search results.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10.html)

[IEdmSearch10 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021