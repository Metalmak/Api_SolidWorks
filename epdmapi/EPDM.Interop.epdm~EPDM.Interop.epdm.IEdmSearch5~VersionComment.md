<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~VersionComment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| VersionComment Property (IEdmSearch5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html) : VersionComment Property (IEdmSearch5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets or sets the version comment substring for which to search.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Property VersionComment As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string VersionComment {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ VersionComment {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

#### Property Value

Substring of version comment for which to search (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

If the search object was obtained using:

* [IEdmVault21::CreateSearch2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault21~CreateSearch2.html) ([IEdmSearch9](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html)), then the version comment may require extended search syntax. (See [Search Syntax](SearchSyntax-epdmapi.html).)

* [IEdmVault5::CreateSearch](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~CreateSearch.html), then the substring for which to search may contain a % wildcard character. For example, **test** searches for all files that have a version comment that contains the word, test.

> % indicates any sequence of characters of any length. You can also use underscore (\_) as a wildcard for exactly one arbitrary character.
>
> To search for strings containing the actual characters '%' and '\_', enclose them in brackets [...]:
>
> > my[\_]text[%]file.txt
>
> You can also enclose the entire string in brackets, because no wildcards occur in it:
>
> > [my\_text%file.txt]

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html)

[IEdmSearch5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2