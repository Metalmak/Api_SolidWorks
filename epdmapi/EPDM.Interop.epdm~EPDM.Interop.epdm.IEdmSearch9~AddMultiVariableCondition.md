<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9~AddMultiVariableCondition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddMultiVariableCondition Method (IEdmSearch9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html) : AddMultiVariableCondition Method (IEdmSearch9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVariableNames*
:   Array of file or folder data card variable names (see **Remarks**)

*bsCondition*
:   Condition to apply to poVariableNames (see **Remarks**)

Adds a multi-variable condition to this search.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddMultiVariableCondition( _    ByVal poVariableNames() As System.String, _    ByVal bsCondition As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddMultiVariableCondition(     System.string[] poVariableNames,    System.string bsCondition ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddMultiVariableCondition(  &   System.array<String^>^ poVariableNames, &   System.String^ bsCondition ) ``` | |

#### Parameters

*poVariableNames*
:   Array of file or folder data card variable names (see **Remarks**)

*bsCondition*
:   Condition to apply to poVariableNames (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSearch9](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IEdmSearch5::GetFirstResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~GetFirstResult.html).

Specify poVariableNames and bsCondition using the basic syntax (single-value search logic rules) as defined in [Search Syntax](SearchSyntax-epdmapi.html).

poVariableNames requires:

* \" to replace each " inside the variable name* \\ to replace each \ inside the variable name* " on both the left and right side of the variable name

poVariableNames supports:

* IDs in place of names* 0 or "" to represent "any variable* \_Name to represent file/folder name

Syntactically incorrect elements in poVariableNames will generate an exception.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9.html)

[IEdmSearch9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2020