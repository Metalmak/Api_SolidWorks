<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~IsLoggedIn.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IsLoggedIn Property (IEdmVault5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : IsLoggedIn Property (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets whether you are logged in to this vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property IsLoggedIn As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsLoggedIn {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool IsLoggedIn {    System.bool get(); } ``` | |

#### Property Value

True if logged in, false if not

# ![](dotnetimages/collapse.gif)Example

[Add Users (C#)](Add_Users_Example_CSharp.htm)

[Add Users (VB.NET)](Add_Users_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Log in to the vault by calling [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) or [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2