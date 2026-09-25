<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~AddVariable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddVariable Method (IEdmSearch5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html) : AddVariable Method (IEdmSearch5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poIdOrName*
:   ID or name of variable for which to search

*poValue*
:   Value for which to search (see **Remarks**)

Obsolete. Superseded by [IEdmSearch8::AddVariable2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8~AddVariable2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddVariable( _    ByRef poIdOrName As System.Object, _    ByRef poValue As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddVariable(     ref System.object poIdOrName,    ref System.object poValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddVariable(  &   System.Object^% poIdOrName, &   System.Object^% poValue ) ``` | |

#### Parameters

*poIdOrName*
:   ID or name of variable for which to search

*poValue*
:   Value for which to search (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

poValue may contain wildcards:

* % - any number of arbitrary characters* \_ - exactly one arbitrary character

The number of times you could call this method was limited to 4 in SOLIDWORKS PDM Professional Version 6.0 and earlier. This restriction was removed in Version 6.1.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_KEY\_NOT\_FOUND: The variable name was not recognized.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html)

[IEdmSearch5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2