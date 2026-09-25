<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetLicense.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetLicense Method (IEdmVault11) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html) : GetLicense Method (IEdmVault11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetLicense*
:   Array of [EdmLicense](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLicense.html) structures; one structure for each license that has one or more users (see **Remarks**)

Gets all of the SOLIDWORKS PDM Professional licenses installed in this vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetLicense( _    ByRef ppoRetLicense() As EdmLicense _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetLicense(     out EdmLicense[] ppoRetLicense ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetLicense(  &   [Out] array<EdmLicense>^ ppoRetLicense ) ``` | |

#### Parameters

*ppoRetLicense*
:   Array of [EdmLicense](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLicense.html) structures; one structure for each license that has one or more users (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

In SOLIDWORKS PDM Professional:

* 2015 SP0 and later, licenses are shared among all vaults that use the same SolidNetwork License Server (SNL). See [IEdmVault14::InstallLicense2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault14~InstallLicense2.html).* 2014 and earlier, licenses were shared among all vaults that were in the same SQL Server instance.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html)

[IEdmVault11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010