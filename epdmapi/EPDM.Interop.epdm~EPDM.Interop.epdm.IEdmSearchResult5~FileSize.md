<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult5~FileSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| FileSize Property (IEdmSearchResult5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearchResult5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult5.html) : FileSize Property (IEdmSearchResult5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the size of this search result.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property FileSize As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int FileSize {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int FileSize {    System.int get(); } ``` | |

#### Property Value

Size of the file; -1 for folders

# ![](dotnetimages/collapse.gif)Remarks

For very large file size search results, use [IEdmSearchResult6::FileSize2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~FileSize2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearchResult5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult5.html)

[IEdmSearchResult5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2