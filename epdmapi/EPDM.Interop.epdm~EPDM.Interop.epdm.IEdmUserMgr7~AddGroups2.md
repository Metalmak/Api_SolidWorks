<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~AddGroups2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddGroups2 Method (IEdmUserMgr7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html) : AddGroups2 Method (IEdmUserMgr7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoGroupData*
:   Array of [EdmGroupData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2.html) structures; one structure for each group

Adds the specified user groups to the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddGroups2( _    ByRef ppoGroupData() As EdmGroupData2 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddGroups2(     out EdmGroupData2[] ppoGroupData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddGroups2(  &   [Out] array<EdmGroupData2>^ ppoGroupData ) ``` | |

#### Parameters

*ppoGroupData*
:   Array of [EdmGroupData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2.html) structures; one structure for each group

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmUserMgr6::AddGroups](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6~AddGroups.html) by providing the ability to specify permissions for added groups.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html)

[IEdmUserMgr7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010