<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6~HasSysRightEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| HasSysRightEx Method (IEdmUserGroup6) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserGroup6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6.html) : HasSysRightEx Method (IEdmUserGroup6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eRight*
:   Permission to check as defined in [EdmSysPerm](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html)

Gets whether this user group has the specified permission.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function HasSysRightEx( _    ByVal eRight As EdmSysPerm _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool HasSysRightEx(     EdmSysPerm eRight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool HasSysRightEx(  &   EdmSysPerm eRight ) ``` | |

#### Parameters

*eRight*
:   Permission to check as defined in [EdmSysPerm](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html)

#### Return Value

True if the user group has the specified permission, false if not

# ![](dotnetimages/collapse.gif)Example

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmUserGroup5::HasSysRight](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5~HasSysRight.html), which checked system permissions represented as bit flags that could be ORed together. As of SOLIDWORKS PDM Professional 2010, new permissions are represented as sequentially numbered constants that cannot be ORed together. You must call this method once for each permission you want to check.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserGroup6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6.html)

[IEdmUserGroup6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010