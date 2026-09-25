<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~GetRevisionNumberComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRevisionNumberComponents Method (IEdmRevisionMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevisionMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr.html) : GetRevisionNumberComponents Method (IEdmRevisionMgr) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoComponents*
:   Array of [EdmRevComponent](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent.html) structures; one structure for each revision number component

Obsolete. Superseded by [IEdmRevisionMgr2::GetRevisionNumberComponents2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2~GetRevisionNumberComponents2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetRevisionNumberComponents( _    ByRef ppoComponents() As EdmRevComponent _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetRevisionNumberComponents(     out EdmRevComponent[] ppoComponents ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetRevisionNumberComponents(  &   [Out] array<EdmRevComponent>^ ppoComponents ) ``` | |

#### Parameters

*ppoComponents*
:   Array of [EdmRevComponent](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent.html) structures; one structure for each revision number component

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr.html)

[IEdmRevisionMgr Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007