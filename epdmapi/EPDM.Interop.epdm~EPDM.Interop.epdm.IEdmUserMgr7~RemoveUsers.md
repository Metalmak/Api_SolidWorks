<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~RemoveUsers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RemoveUsers Method (IEdmUserMgr7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html) : RemoveUsers Method (IEdmUserMgr7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poUserIDs*
:   Array of IDs of the users to remove (see **Remarks**)

Removes the specified users from the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub RemoveUsers( _    ByVal poUserIDs() As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void RemoveUsers(     System.int[] poUserIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RemoveUsers(  &   System.array<int>^ poUserIDs ) ``` | |

#### Parameters

*poUserIDs*
:   Array of IDs of the users to remove (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you specify an ID in poUserIDs that does not exist, it is ignored.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The logged-in user lacks the [EdmSysPerm](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html).EdmSysPerm\_EditUserMgr permission.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html)

[IEdmUserMgr7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010