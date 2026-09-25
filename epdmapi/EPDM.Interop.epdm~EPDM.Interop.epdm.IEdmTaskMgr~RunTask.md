<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskMgr~RunTask.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RunTask Method (IEdmTaskMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskMgr.html) : RunTask Method (IEdmTaskMgr) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oTask*
:   Task add-in to run as defined by [EdmTaskInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskInfo.html)

*poSelections*
:   Array of [EdmSelItem2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2.html)

*lParentWnd*
:   Parent window

Runs the specified task add-in.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub RunTask( _    ByVal oTask As EdmTaskInfo, _    ByVal poSelections() As EdmSelItem2, _    ByVal lParentWnd As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void RunTask(     EdmTaskInfo oTask,    EdmSelItem2[] poSelections,    System.int lParentWnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RunTask(  &   EdmTaskInfo oTask, &   array<EdmSelItem2>^ poSelections, &   System.int lParentWnd ) ``` | |

#### Parameters

*oTask*
:   Task add-in to run as defined by [EdmTaskInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskInfo.html)

*poSelections*
:   Array of [EdmSelItem2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2.html)

*lParentWnd*
:   Parent window

# ![](dotnetimages/collapse.gif)Example

See the [IEdmTaskMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskMgr.html) example.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskMgr.html)

[IEdmTaskMgr Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018 SP04