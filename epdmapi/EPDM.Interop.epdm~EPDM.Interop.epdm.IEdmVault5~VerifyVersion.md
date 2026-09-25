<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~VerifyVersion.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| VerifyVersion Method (IEdmVault5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : VerifyVersion Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lMajor*
:   Minimum major version number

*lMinor*
:   Minimum minor version number

Verifies that the installed SOLIDWORKS PDM Professional is at the specified version level or higher.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub VerifyVersion( _    ByVal lMajor As System.Integer, _    ByVal lMinor As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void VerifyVersion(     System.int lMajor,    System.int lMinor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void VerifyVersion(  &   System.int lMajor, &   System.int lMinor ) ``` | |

#### Parameters

*lMajor*
:   Minimum major version number

*lMinor*
:   Minimum minor version number

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Add-ins that depend on a specific SOLIDWORKS PDM Professional version should make themselves impossible to install on earlier versions of SOLIDWORKS PDM Professional. To do this, set the minimum version of SOLIDWORKS PDM Professional in mlRequiredVersionMajor and mlRequiredVersionMinor of the [EdmAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo.html) structure that is passed as a parameter in [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_UNSUPPORTED\_PROGRAM\_VERSION: The installed program is at a version level that is lower than the specified version.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2