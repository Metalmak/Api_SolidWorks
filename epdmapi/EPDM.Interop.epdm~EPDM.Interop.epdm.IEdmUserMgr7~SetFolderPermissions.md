<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~SetFolderPermissions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetFolderPermissions Method (IEdmUserMgr7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html) : SetFolderPermissions Method (IEdmUserMgr7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPermissions*
:   Array of [EdmFolderPermission](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission.html) structures; one structure for each permission assignment

Sets specified permissions on a specified folder for a specified user or group.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetFolderPermissions( _    ByVal poPermissions() As EdmFolderPermission _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFolderPermissions(     EdmFolderPermission[] poPermissions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFolderPermissions(  &   array<EdmFolderPermission>^ poPermissions ) ``` | |

#### Parameters

*poPermissions*
:   Array of [EdmFolderPermission](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission.html) structures; one structure for each permission assignment

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUserMgr7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The logged-in user lacks the [EdmSysPerm](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html).EdmSysPerm\_EditUserMgr permission.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html)

[IEdmUserMgr7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010