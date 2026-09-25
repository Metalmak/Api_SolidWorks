<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5~SetGroupRights.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetGroupRights Method (IEdmFolderData5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolderData5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html) : SetGroupRights Method (IEdmFolderData5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lGroupID*
:   ID of user group for which to set permissions

*lEdmRightFlags*
:   Combination of [EdmRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRightFlags.html) bits

Sets the specified permissions for the specified user group.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetGroupRights( _    ByVal lGroupID As System.Integer, _    ByVal lEdmRightFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetGroupRights(     System.int lGroupID,    System.int lEdmRightFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetGroupRights(  &   System.int lGroupID, &   System.int lEdmRightFlags ) ``` | |

#### Parameters

*lGroupID*
:   ID of user group for which to set permissions

*lEdmRightFlags*
:   Combination of [EdmRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRightFlags.html) bits

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFolderData5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Retrieve user groups using [IEdmUserMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolderData5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html)

[IEdmFolderData5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2