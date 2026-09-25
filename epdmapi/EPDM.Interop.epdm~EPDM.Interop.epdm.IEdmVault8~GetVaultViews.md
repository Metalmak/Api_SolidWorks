<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8~GetVaultViews.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetVaultViews Method (IEdmVault8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8.html) : GetVaultViews Method (IEdmVault8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetViews*
:   Array of [EdmViewInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo.html) structures; one structure for each view

*bOnlyLoggedIn*
:   True to get views in which you are currently logged, false to get all views

Gets all of the views set up on this vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetVaultViews( _    ByRef ppoRetViews() As EdmViewInfo, _    ByVal bOnlyLoggedIn As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetVaultViews(     out EdmViewInfo[] ppoRetViews,    System.bool bOnlyLoggedIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetVaultViews(  &   [Out] array<EdmViewInfo>^ ppoRetViews, &   System.bool bOnlyLoggedIn ) ``` | |

#### Parameters

*ppoRetViews*
:   Array of [EdmViewInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo.html) structures; one structure for each view

*bOnlyLoggedIn*
:   True to get views in which you are currently logged, false to get all views

# ![](dotnetimages/collapse.gif)Example

See the [IEdmVault8](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

You do not have to call [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) or [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html) before calling this method.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8.html)

[IEdmVault8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4