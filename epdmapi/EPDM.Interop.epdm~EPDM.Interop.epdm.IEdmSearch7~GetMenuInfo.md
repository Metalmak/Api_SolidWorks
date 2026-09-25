<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch7~GetMenuInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetMenuInfo Method (IEdmSearch7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch7.html) : GetMenuInfo Method (IEdmSearch7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoForms*
:   Array of search forms

*ppoFavorites*
:   Array of favorite searches

*plSysPerm*
:   Combination of [EdmSysRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html) bits for the logged-in user

*plEdmGetMenuInfoFlags*
:   Combination of [EdmGetMenuInfoFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetMenuInfoFlags.html) bits

Gets information that can be used to display a quick launch menu from which the user can start the search tool and activate one of his search forms or favorites.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetMenuInfo( _    ByRef ppoForms() As System.String, _    ByRef ppoFavorites() As System.String, _    ByRef plSysPerm As System.Integer, _    ByRef plEdmGetMenuInfoFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetMenuInfo(     out System.string[] ppoForms,    out System.string[] ppoFavorites,    out System.int plSysPerm,    out System.int plEdmGetMenuInfoFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetMenuInfo(  &   [Out] System.array<String^>^ ppoForms, &   [Out] System.array<String^>^ ppoFavorites, &   [Out] System.int plSysPerm, &   [Out] System.int plEdmGetMenuInfoFlags ) ``` | |

#### Parameters

*ppoForms*
:   Array of search forms

*ppoFavorites*
:   Array of favorite searches

*plSysPerm*
:   Combination of [EdmSysRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html) bits for the logged-in user

*plEdmGetMenuInfoFlags*
:   Combination of [EdmGetMenuInfoFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetMenuInfoFlags.html) bits

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch7.html)

[IEdmSearch7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009