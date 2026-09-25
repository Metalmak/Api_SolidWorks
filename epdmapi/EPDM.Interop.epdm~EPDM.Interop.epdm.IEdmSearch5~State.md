<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~State.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| State Property (IEdmSearch5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html) : State Property (IEdmSearch5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets or sets the ID or name of the workflow state in which to search.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Property State As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object State {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ State {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

#### Property Value

ID or name of the workflow state in which to search

# ![](dotnetimages/collapse.gif)Remarks

If the search object was obtained using:

* [IEdmVault21::CreateSearch2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault21~CreateSearch2.html) ([IEdmSearch9](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html)), then the workflow state name may require extended search syntax. (See [Search Syntax](SearchSyntax-epdmapi.html).)

* [IEdmVault5::CreateSearch](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~CreateSearch.html), then the workflow state name for which to search may contain a % wildcard character. For example, **test** searches for all files that have a workflow state that contains the word, test.
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

[IEdmSearch5::FindHistoricStates Property ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~FindHistoricStates.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2