<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault19~GetRevisionTableSettings.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRevisionTableSettings Method (IEdmVault19) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault19 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault19.html) : GetRevisionTableSettings Method (IEdmVault19) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*vbManagedInPDM*
:   True if the revision table is managed by PDM Professional, false if managed by SOLIDWORKS

*plNoOfRows*
:   Number of visible rows in the revision table

*vbRevTableOrder*
:   True if the revision table order is ascending, false if descending

*pbsRevPlaceholder*
:   Revision table placeholder character

Gets the settings for revision tables of drawings in this vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetRevisionTableSettings( _    ByRef vbManagedInPDM As System.Boolean, _    ByRef plNoOfRows As System.Integer, _    ByRef vbRevTableOrder As System.Boolean, _    ByRef pbsRevPlaceholder As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetRevisionTableSettings(     out System.bool vbManagedInPDM,    out System.int plNoOfRows,    out System.bool vbRevTableOrder,    out System.string pbsRevPlaceholder ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetRevisionTableSettings(  &   [Out] System.bool vbManagedInPDM, &   [Out] System.int plNoOfRows, &   [Out] System.bool vbRevTableOrder, &   [Out] System.String^ pbsRevPlaceholder ) ``` | |

#### Parameters

*vbManagedInPDM*
:   True if the revision table is managed by PDM Professional, false if managed by SOLIDWORKS

*plNoOfRows*
:   Number of visible rows in the revision table

*vbRevTableOrder*
:   True if the revision table order is ascending, false if descending

*pbsRevPlaceholder*
:   Revision table placeholder character

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault19 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault19.html)

[IEdmVault19 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault19_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018