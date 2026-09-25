<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~GetFolderPermissions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFolderPermissions Method (IEdmUserMgr7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html) : GetFolderPermissions Method (IEdmUserMgr7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lOwnerID*
:   ID of the user or group for which to get permissions; 0 to return permissions for all users and groups

*meOwnerType*
:   Type of lOwnerID as defined in [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html)

*lFolderID*
:   ID of folder for which to get permissions

*lEdmGetPermFlags*
:   Combination of [EdmGetPermFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetPermFlag.html) bits (see **Remarks**)

*ppoPermissions*
:   Array of [EdmFolderPermission](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission.html) structures; one structure for each permission

Gets the permissions set on the specified folder for the specified user or group.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetFolderPermissions( _    ByVal lOwnerID As System.Integer, _    ByVal meOwnerType As EdmObjectType, _    ByVal lFolderID As System.Integer, _    ByVal lEdmGetPermFlags As System.Integer, _    ByRef ppoPermissions() As EdmFolderPermission _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFolderPermissions(     System.int lOwnerID,    EdmObjectType meOwnerType,    System.int lFolderID,    System.int lEdmGetPermFlags,    out EdmFolderPermission[] ppoPermissions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFolderPermissions(  &   System.int lOwnerID, &   EdmObjectType meOwnerType, &   System.int lFolderID, &   System.int lEdmGetPermFlags, &   [Out] array<EdmFolderPermission>^ ppoPermissions ) ``` | |

#### Parameters

*lOwnerID*
:   ID of the user or group for which to get permissions; 0 to return permissions for all users and groups

*meOwnerType*
:   Type of lOwnerID as defined in [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html)

*lFolderID*
:   ID of folder for which to get permissions

*lEdmGetPermFlags*
:   Combination of [EdmGetPermFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetPermFlag.html) bits (see **Remarks**)

*ppoPermissions*
:   Array of [EdmFolderPermission](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission.html) structures; one structure for each permission

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUserMgr7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method returns not only permissions explicitly set on a folder, but also permissions inherited from parent folders, depending on the combination of EdmGetPermFlag bits in lEdmGetPermFlags.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html)

[IEdmUserMgr7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010