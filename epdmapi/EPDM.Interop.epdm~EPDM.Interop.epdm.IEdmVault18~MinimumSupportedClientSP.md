<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault18~MinimumSupportedClientSP.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| MinimumSupportedClientSP Property (IEdmVault18) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault18 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault18.html) : MinimumSupportedClientSP Property (IEdmVault18) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the minimum client service pack supported by this vault's views.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property MinimumSupportedClientSP As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int MinimumSupportedClientSP {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int MinimumSupportedClientSP {    System.int get(); } ``` | |

#### Property Value

Minimum supported client service pack (e.g., 0, 1, 2, 3, 4, 5)

# ![](dotnetimages/collapse.gif)Remarks

As of SOLIDWORKS PDM Professional 2017 SP01, client/server minor version mismatches are supported. For example, if this method returns "0", then for the current major version (e.g., 2017), an SP0 client machine works with vault views created with other service packs.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault18 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault18.html)

[IEdmVault18 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault18_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017 SP01