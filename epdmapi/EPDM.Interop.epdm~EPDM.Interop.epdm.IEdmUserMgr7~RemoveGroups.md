<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~RemoveGroups.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RemoveGroups Method (IEdmUserMgr7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html) : RemoveGroups Method (IEdmUserMgr7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poGroupIDs*
:   Array of IDs of the groups to remove (see **Remarks**)

Removes the specified groups from the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub RemoveGroups( _    ByVal poGroupIDs() As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void RemoveGroups(     System.int[] poGroupIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RemoveGroups(  &   System.array<int>^ poGroupIDs ) ``` | |

#### Parameters

*poGroupIDs*
:   Array of IDs of the groups to remove (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you specify an ID in poGroupIDs that does not exist, it is ignored.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The logged-in user lacks the [EdmSysPerm](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html).EdmSysPerm\_EditUserMgr permission.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html)

[IEdmUserMgr7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010