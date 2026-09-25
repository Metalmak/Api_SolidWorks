<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5~HasSysRight.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| HasSysRight Method (IEdmUserGroup5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserGroup5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5.html) : HasSysRight Method (IEdmUserGroup5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eRight*
:   Combination of [EdmSysRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html)

Obsolete. Superseded by [IEdmUserGroup6::HasSysRightEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6~HasSysRightEx.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function HasSysRight( _    ByVal eRight As EdmSysRightFlags _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool HasSysRight(     EdmSysRightFlags eRight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool HasSysRight(  &   EdmSysRightFlags eRight ) ``` | |

#### Parameters

*eRight*
:   Combination of [EdmSysRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html)

#### Return Value

True if the user group has all the permissions, false if not

# ![](dotnetimages/collapse.gif)Remarks

This method is superseded by [IEdmUserGroup6::HasSysRightEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6~HasSysRightEx.html).

Before SOLIDWORKS PDM Professional 2010, IEdmUserGroup5::HasSysRight supported the bit-wise combination of system permissions. Because the number of system permissions has grown, and they do not all fit in a 32-bit integer, system permissions added in SOLIDWORKS PDM Professional 2010 and later are sequential numeric constants instead of bit flags. You must use IEdmUserGroup6::HasSysRightEx to check permissions added in SOLIDWORKS PDM Professional 2010 and later.

To check individual user permissions, call [IEdmUser5::HasSysRight](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5~HasSysRight.html), which checks both permissions set directly on the user and permissions inherited from groups of which he is a member.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed, and all of the permissions are set.* S\_FALSE: The method successfully executed, but one or more of the permissions are not set.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserGroup5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5.html)

[IEdmUserGroup5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional version 5.2