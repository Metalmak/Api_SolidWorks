<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5~CheckPermission.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CheckPermission Method (IEdmTransition5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTransition5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5.html) : CheckPermission Method (IEdmTransition5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets whether the logged-in user has permission to perform this transition.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CheckPermission() As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CheckPermission() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CheckPermission(); ``` | |

#### Return Value

True if the user can make this transition, false if not

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The user lacks permission.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTransition5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5.html)

[IEdmTransition5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2