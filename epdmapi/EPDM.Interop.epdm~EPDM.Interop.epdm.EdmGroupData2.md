<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2.html -->

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

| EdmGroupData2 Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGroupData2 Structure |

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
| ``` Public Structure EdmGroupData2     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmGroupData2 : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmGroupData2 : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmGroupData2{
  string [mbsName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2~mbsName.html);
  string [mbsDescription](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2~mbsDescription.html);
  integer [mlFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2~mlFlags.html);
  array([enum EdmSysPerm](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html)) [moSysPerms](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2~moSysPerms.html);
  short [mbAutoAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2~mbAutoAdd.html);
  array(integer) [moMembers](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2~moMembers.html);
  integer [mlGroupID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2~mlGroupID.html);
  integer [mhStatus](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2~mhStatus.html);
  [IEdmUserGroup5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5.html) \*[mpoGroup](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2~mpoGroup.html);
};

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This structure extends [EdmGroupData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData.html) and is used in [IEdmUserMgr7::AddGroups2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~AddGroups2.html) to add user groups to the vault.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmGroupData2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData2_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010