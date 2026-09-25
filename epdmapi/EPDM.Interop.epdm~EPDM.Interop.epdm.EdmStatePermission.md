<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStatePermission.html -->

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

| EdmStatePermission Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStatePermission_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmStatePermission Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains state permission information.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmStatePermission     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmStatePermission : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmStatePermission : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmStatePermission
{
  [enum EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) [meOwnerType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStatePermission~meOwnerType.html);
  integer [mlOwnerID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStatePermission~mlOwnerID.html);
  integer [mlStateID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStatePermission~mlStateID.html);
  integer [mlEdmRightFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStatePermission~mlEdmRightFlag.html);

};

# ![](dotnetimages/collapse.gif)Remarks

Used by [IEdmUserMgr9::GetStatePermissions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9~GetStatePermissions.html) and [IEdmUserMgr9::SetStatePermissions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9~SetStatePermissions.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmStatePermission Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStatePermission_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017