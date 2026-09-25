<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9~GetTransitionPermissions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetTransitionPermissions Method (IEdmUserMgr9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9.html) : GetTransitionPermissions Method (IEdmUserMgr9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lOwnerID*
:   ID of the user or group for which to get permissions; 0 to return permissions for all users and groups

*meOwnerType*
:   Type of lOwnerID as defined in [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html); valid only if lOwnerID is not 0

*lTransitionID*
:   ID of transition for which to get permissions; 0 to return permissions for all transitions

*ppoPermissions*
:   Array of [EdmTransitionPermission](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission.html) structures; one structure for each permission assignment

Gets the transition permissions for the specified owner and transition.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetTransitionPermissions( _    ByVal lOwnerID As System.Integer, _    ByVal meOwnerType As EdmObjectType, _    ByVal lTransitionID As System.Integer, _    ByRef ppoPermissions() As EdmTransitionPermission _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetTransitionPermissions(     System.int lOwnerID,    EdmObjectType meOwnerType,    System.int lTransitionID,    out EdmTransitionPermission[] ppoPermissions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetTransitionPermissions(  &   System.int lOwnerID, &   EdmObjectType meOwnerType, &   System.int lTransitionID, &   [Out] array<EdmTransitionPermission>^ ppoPermissions ) ``` | |

#### Parameters

*lOwnerID*
:   ID of the user or group for which to get permissions; 0 to return permissions for all users and groups

*meOwnerType*
:   Type of lOwnerID as defined in [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html); valid only if lOwnerID is not 0

*lTransitionID*
:   ID of transition for which to get permissions; 0 to return permissions for all transitions

*ppoPermissions*
:   Array of [EdmTransitionPermission](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission.html) structures; one structure for each permission assignment

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUserMgr9](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9.html)

[IEdmUserMgr9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9_members.html)

[IEdmUserMgr9::SetTransitionPermissions Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9~SetTransitionPermissions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017