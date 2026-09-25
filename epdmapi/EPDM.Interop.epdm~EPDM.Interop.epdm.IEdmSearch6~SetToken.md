<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6~SetToken.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetToken Method (IEdmSearch6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6.html) : SetToken Method (IEdmSearch6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eTok*
:   Search token for which to set a value as defined in [EdmSearchToken](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSearchToken.html) (see **Remarks)**

*oValue*
:   New value for token

Sets the specified token with the specified value.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetToken( _    ByVal eTok As EdmSearchToken, _    ByVal oValue As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetToken(     EdmSearchToken eTok,    System.object oValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetToken(  &   EdmSearchToken eTok, &   System.Object^ oValue ) ``` | |

#### Parameters

*eTok*
:   Search token for which to set a value as defined in [EdmSearchToken](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSearchToken.html) (see **Remarks)**

*oValue*
:   New value for token

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSearch6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6.html) and [IEdmSearch9](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

For every search you must explicitly set EdmSearchToken.Edmstok\_AllVersions to either true or false. If you leave it unset, unexpected search results can occur.

If the search object was obtained using [IEdmVault21::CreateSearch2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault21~CreateSearch2.html) (IEdmSearch9), then oValue may contain extended search syntax. (See [Search Syntax](SearchSyntax-epdmapi.html).)

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6.html)

[IEdmSearch6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007