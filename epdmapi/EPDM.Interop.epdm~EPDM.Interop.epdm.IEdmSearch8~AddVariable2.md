<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8~AddVariable2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddVariable2 Method (IEdmSearch8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8.html) : AddVariable2 Method (IEdmSearch8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poIdOrName*
:   ID or name of variable for which to search

*poValue*
:   Value or regular expression for which to search (see **Remarks**)

*lEdmVarOp*
:   Operator to apply to poValue as defined in [EdmVarOp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarOp.html) (see **Remarks**)

Adds a file or folder data card variable to this search.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddVariable2( _    ByRef poIdOrName As System.Object, _    ByRef poValue As System.Object, _    Optional ByVal lEdmVarOp As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddVariable2(     ref System.object poIdOrName,    ref System.object poValue,    System.int lEdmVarOp ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddVariable2(  &   System.Object^% poIdOrName, &   System.Object^% poValue, &   System.int lEdmVarOp ) ``` | |

#### Parameters

*poIdOrName*
:   ID or name of variable for which to search

*poValue*
:   Value or regular expression for which to search (see **Remarks**)

*lEdmVarOp*
:   Operator to apply to poValue as defined in [EdmVarOp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarOp.html) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSearch8](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8.html) and [IEdmSearch9](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

If the search object:

* is [IEdmSearch5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html), then:
  + before calling this method, call [IEdmSearch8::BeginAND](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8~BeginAND.html) or [IEdmSearch8::BeginOR](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8~BeginOR.html) to construct more complicated search criteria.+ poValue may contain wildcards:

> * % - any number of arbitrary characters* \_  - exactly one arbitrary character

* is created using [IEdmVault21::CreateSearch2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault21~CreateSearch2.html) (IEdmSearch9), then poValue follows basic syntax (single-value search logic rules. See [Search Syntax](SearchSyntax-epdmapi.html).) lEdmVarOp must be Nothing or null.

The number of times you could call this method was limited to 4 in SOLIDWORKS PDM Professional Version 6.0 and earlier. This restriction was removed in Version 6.1.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_KEY\_NOT\_FOUND: The variable name was not recognized.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8.html)

[IEdmSearch8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018