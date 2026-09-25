<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5~HasSysRight.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| HasSysRight Method (IEdmUser5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUser5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5.html) : HasSysRight Method (IEdmUser5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eRight*
:   Permissions as defined in [EdmSysRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html)

Obsolete. Superseded by [IEdmUser7::HasSysRightEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser7~HasSysRightEx.html).

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
:   Permissions as defined in [EdmSysRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html)

#### Return Value

True if the user has all of the permissions, false if the user lacks one or more of the permissions

# ![](dotnetimages/collapse.gif)Remarks

This method is superseded by [IEdmUser7::HasSysRightEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser7~HasSysRightEx.html).

Before SOLIDWORKS PDM Professional 2010, IEdmUser5::HasSysRight supported the bit-wise combination of system permissions. Because the number of system permissions has grown, and they do not all fit in a 32-bit integer, system permissions added in SOLIDWORKS PDM Professional 2010 and later are sequential numeric constants instead of bit flags. You must use IEdmUser7::HasSysRightEx to check permissions added in SOLIDWORKS PDM Professional 2010 and later.

This method checks both the permissions set directly on the user and the permissions inherited from the groups of which the user is a member.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The method successfully executed, but the user lacks the specified permissions.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUser5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5.html)

[IEdmUser5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2