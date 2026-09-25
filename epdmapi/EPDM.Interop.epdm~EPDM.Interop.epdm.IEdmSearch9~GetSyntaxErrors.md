<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9~GetSyntaxErrors.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetSyntaxErrors Method (IEdmSearch9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html) : GetSyntaxErrors Method (IEdmSearch9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets syntax errors resulting from this search.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetSyntaxErrors() As System.String() ``` | |

| C# |  |
| --- | --- |
| ``` System.string[] GetSyntaxErrors() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.array<String^>^ GetSyntaxErrors(); ``` | |

#### Return Value

Array of localized syntax errors; Nothing or null if no errors

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSearch9](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method returns errors only if the advanced specifier (@:) is specified at the beginning of search syntax conditions.

If [IEdmSearch5::GetFirstResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~GetFirstResult.html) returns Nothing or null it can mean either:

* the search found no documents

    - or -

* there were one or more search syntax errrors.

Call this method after IEdmSearch5::GetFirstResult to determine whether there are syntax errors. If this method returns Nothing or null, then you can assume that IEdmSearch5::GetFirstResult found no documents.

See [Search Syntax](SearchSyntax-epdmapi.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html)

[IEdmSearch9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2020