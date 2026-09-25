<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition9~UserPartOfTransitionRoles.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| UserPartOfTransitionRoles Property (IEdmTransition9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTransition9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition9.html) : UserPartOfTransitionRoles Property (IEdmTransition9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lProjectID*
:   Project ID

Gets whether the logged-in user has a role in this parallel transition.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property UserPartOfTransitionRoles( _    ByVal lProjectID As System.Integer _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UserPartOfTransitionRoles(     System.int lProjectID ) {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool UserPartOfTransitionRoles {    System.bool get(System.int lProjectID); } ``` | |

#### Parameters

*lProjectID*
:   Project ID

#### Property Value

True if the logged-in user has a role in this parallel transition, false if not

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTransition9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition9.html)

[IEdmTransition9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition9_members.html)