<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile11~PrivateStateFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| PrivateStateFile Property (IEdmFile11) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile11.html) : PrivateStateFile Property (IEdmFile11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets whether this file is in a private state.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property PrivateStateFile As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool PrivateStateFile {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool PrivateStateFile {    System.bool get(); } ``` | |

#### Property Value

True if this file is in a private state, false if not

# ![](dotnetimages/collapse.gif)Example

[Add Files to Vault (VB.NET)](Add_Files_to_Vault_Example_VBNET.htm)

[Add Files to Vault (C#)](Add_Files_to_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Files in a private state:

* are accessible only to the user adding them and the SOLIDWORKS PDM Professional Admin user.* have no assigned workflow or category.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile11.html)

[IEdmFile11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile11_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015 SP02