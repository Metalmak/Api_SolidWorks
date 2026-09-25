<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission.html -->

![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/drpdown.gif)
![](dotnetimages/drpdown_orange.gif)
![](dotnetimages/copycode.gif)
![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |

| EdmFolderPermission Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmFolderPermission Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains permission settings.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmFolderPermission     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmFolderPermission : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmFolderPermission : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmFolderPermission
{
  integer [mlEdmRightFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission~mlEdmRightFlag.html);
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission~mlFolderID.html);
  integer [mlOwnerID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission~mlOwnerID.html);
  [enum EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) [meOwnerType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission~meOwnerType.html);
};

# ![](dotnetimages/collapse.gif)Example

[Get and Set Folder Permissions (VB.NET)](Get_and_Set_Folder_Permissions_Example_VBNET.htm)

[Get and Set Folder Permissions (C#)](Get_and_Set_Folder_Permissions_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Used by [IEdmUserMgr7::GetFolderPermissions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~GetFolderPermissions.html) and [IEdmUserMgr7::SetFolderPermissions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~SetFolderPermissions.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmFolderPermission Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderPermission_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010