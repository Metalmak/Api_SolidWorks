<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetVersion.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetVersion Method (IEdmVault5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : GetVersion Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*plMajor*
:   Major version number

*plMinor*
:   Minor version number

Gets the version of SOLIDWORKS PDM Professional that is installed on this machine.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetVersion( _    ByRef plMajor As System.Integer, _    ByRef plMinor As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetVersion(     out System.int plMajor,    out System.int plMinor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetVersion(  &   [Out] System.int plMajor, &   [Out] System.int plMinor ) ``` | |

#### Parameters

*plMajor*
:   Major version number

*plMinor*
:   Minor version number

# ![](dotnetimages/collapse.gif)Example

[Log Into Vault and Display Information (C#)](Log_Into_Vault_and_Display_Information_Example_CSharp.htm)

[Log Into Vault and Display Information (VB.NET)](Log_Into_Vault_and_Display_Information_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

You do not need to call [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) or [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html) before calling this method.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2