<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault15~GetClientLog.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetClientLog Method (IEdmVault15) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault15 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault15.html) : GetClientLog Method (IEdmVault15) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*pbsRetLogs*
:   Contents of the current user's log

Gets the contents of the current user's log.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetClientLog( _    ByRef pbsRetLogs As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetClientLog(     out System.string pbsRetLogs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetClientLog(  &   [Out] System.String^ pbsRetLogs ) ``` | |

#### Parameters

*pbsRetLogs*
:   Contents of the current user's log

# ![](dotnetimages/collapse.gif)Example

[Traverse Folders and Files in Vault (VB.NET)](Traverse_Folders_and_Files_in_Vault_Example_VBNET.htm)

[Traverse Folders and Files in Vault (C#)](Traverse_Folders_and_Files_in_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The current user's log appears when you click **SOLIDWORKS PDM Administration > Local Settings > Log File** in the SOLIDWORKS PDM Administration Tool. This method returns the full log.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault15 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault15.html)

[IEdmVault15 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault15_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015 SP03