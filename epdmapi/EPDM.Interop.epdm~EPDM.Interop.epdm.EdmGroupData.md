<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData.html -->

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

| EdmGroupData Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGroupData Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a user group.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmGroupData     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmGroupData : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmGroupData : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmGroupData

{
  string [mbsName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData~mbsName.html);

  string [mbsDescription](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData~mbsDescription.html);

integer [mlFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData~mlFlags.html);

integer [mlSysRights](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData~mlSysRights.html);

short [mbAutoAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData~mbAutoAdd.html);

array [moMembers](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData~moMembers.html);

integer [mlGroupID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData~mlGroupID.html);

integer [mhStatus](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData~mhStatus.html);

  [IEdmUserGroup5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5.html) \*[mpoGroup](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData~mpoGroup.html);
};

# ![](dotnetimages/collapse.gif)Remarks

Used in [IEdmUserMgr6::AddGroups](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6~AddGroups.html). This structure is extended by [EdmGroupData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2.html), which should be used instead of this structure in version 2010 and later.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmGroupData Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007