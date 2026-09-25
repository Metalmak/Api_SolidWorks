<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition8~CheckProjectPermission.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CheckProjectPermission Method (IEdmTransition8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTransition8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition8.html) : CheckProjectPermission Method (IEdmTransition8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lProjectID*
:   Project ID

Checks whether the user has permission to perform this transition for the specified project.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CheckProjectPermission( _    ByVal lProjectID As System.Integer _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CheckProjectPermission(     System.int lProjectID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CheckProjectPermission(  &   System.int lProjectID ) ``` | |

#### Parameters

*lProjectID*
:   Project ID

#### Return Value

True if the user has permission to perform the transition, false if not

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTransition8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition8.html)

[IEdmTransition8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition8_members.html)