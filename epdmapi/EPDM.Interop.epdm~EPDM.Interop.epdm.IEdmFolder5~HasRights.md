<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRights.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| HasRights Method (IEdmFolder5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : HasRights Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lRights*
:   Combination of [EdmRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRightFlags.html) bits

*plFileID*
:   ID of file to check

Obsolete. Superseded by [IEdmFolder5::HasRightsEx.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRightsEx.html)

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub HasRights( _    ByVal lRights As System.Integer, _    ByRef plFileID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void HasRights(     System.int lRights,    ref System.int plFileID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void HasRights(  &   System.int lRights, &   System.int% plFileID ) ``` | |

#### Parameters

*lRights*
:   Combination of [EdmRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRightFlags.html) bits

*plFileID*
:   ID of file to check

# ![](dotnetimages/collapse.gif)Remarks

This method is superseded by [IEdmFolder5::HasRightsEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRightsEx.html), which provides the ability to check rights on just this folder. Programs that do not need backwards compatibility with SOLIDWORKS PDM Professional 5.2 should use the new method.

This method takes into account both the rights set explicitly on the user and those rights that are inherited from groups of which the user is a member.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The user lacks one or more of the specified rights.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2