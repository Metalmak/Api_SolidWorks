<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission.html -->

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

| EdmTransitionPermission Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmTransitionPermission Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains transition permission information.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmTransitionPermission     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmTransitionPermission : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmTransitionPermission : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmTransitionPermission
{
  [enum EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) [meOwnerType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission~meOwnerType.html);
  integer [mlOwnerID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission~mlOwnerID.html);
  integer [mlTransitionID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission~mlTransitionID.html);
  integer [mlEdmRightFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission~mlEdmRightFlag.html);

};

# ![](dotnetimages/collapse.gif)Remarks

Used by [IEdmUserMgr9::GetTransitionPermissions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9~GetTransitionPermissions.html) and [IEdmUserMgr9::SetTransitionPermissions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9~SetTransitionPermissions.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmTransitionPermission Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017