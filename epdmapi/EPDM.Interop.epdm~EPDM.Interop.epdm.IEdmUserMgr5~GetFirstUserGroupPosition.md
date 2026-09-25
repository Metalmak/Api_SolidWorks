<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5~GetFirstUserGroupPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstUserGroupPosition Method (IEdmUserMgr5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html) : GetFirstUserGroupPosition Method (IEdmUserMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of the user groups in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstUserGroupPosition() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstUserGroupPosition() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstUserGroupPosition(); ``` | |

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the first user group in the enumeration

# ![](dotnetimages/collapse.gif)Example

[Get and Set Folder Permissions (VB.NET)](Get_and_Set_Folder_Permissions_Example_VBNET.htm)

[Get and Set Folder Permissions (C#)](Get_and_Set_Folder_Permissions_Example_CSharp.htm)

[Traverse Users and Groups in Vault (C#)](Traverse_Users_and_Groups_in_Vault_Example_CSharp.htm)

[Traverse Users and Groups in Vault (VB.NET)](Traverse_Users_and_Groups_in_Vault_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, pass the returned position of the first user group to [IEdmUserMgr5::GetNextUserGroup](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5~GetNextUserGroup.html) to get the first user group in this list. Then call IEdmUserMgr5::GetNextUserGroup repeatedly to get the rest of the user groups.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html)

[IEdmUserMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2