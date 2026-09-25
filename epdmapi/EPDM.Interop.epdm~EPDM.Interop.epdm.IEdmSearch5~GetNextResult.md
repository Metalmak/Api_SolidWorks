<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~GetNextResult.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextResult Method (IEdmSearch5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html) : GetNextResult Method (IEdmSearch5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the next file or folder that matches the search criteria.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextResult() As IEdmSearchResult5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmSearchResult5 GetNextResult() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmSearchResult5^ GetNextResult(); ``` | |

#### Return Value

[IEdmSearchResult5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult5.html); Nothing or null if no more files or folders match the search criteria

# ![](dotnetimages/collapse.gif)Example

See the examples for [IEdmSearch5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html) and [IEdmSearch10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10.html).

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IEdmSearch5::GetFirstResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~GetFirstResult.html) or [IEdmSearch10::GetFirstFavoriteResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10~GetFirstFavoriteResult.html) to retrieve the first file or folder that matches the search criteria.

C++ users must release the returned interface, IEdmSearchResult5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The method successfully executed, but no files or folders match the search criteria.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html)

[IEdmSearch5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2