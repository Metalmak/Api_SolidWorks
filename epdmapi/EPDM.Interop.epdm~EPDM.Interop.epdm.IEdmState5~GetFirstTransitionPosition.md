<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~GetFirstTransitionPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstTransitionPosition Method (IEdmState5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html) : GetFirstTransitionPosition Method (IEdmState5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bExitTransitions*
:   Optionally true to enumerate the transitions from this workflow state, false to enumerate the transition to this workflow state; default is true

Starts an enumeration of the transitions to and from this workflow state.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstTransitionPosition( _    Optional ByVal bExitTransitions As System.Boolean _ ) As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstTransitionPosition(     System.bool bExitTransitions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstTransitionPosition(  &   System.bool bExitTransitions ) ``` | |

#### Parameters

*bExitTransitions*
:   Optionally true to enumerate the transitions from this workflow state, false to enumerate the transition to this workflow state; default is true

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position in the list of the first transition to or from this workflow state (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Get File's State Transitions (C#)](Get_Files_State_Transitions_Example_CSharp.htm)

[Get File's State Transitions (VB.NET)](Get_Files_State_Transitions_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, pass the returned position of the first transition to or from this workflow state to [IEdmState5::GetNextTransition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~GetNextTransition.html) to get the first transition to or from this workflow state. Then call IEdmState5::GetNextTransition repeatedly to get the rest of the transitions to and from this workflow state.

C++ programmers not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html)

[IEdmState5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2