<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~GetNextTransition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextTransition Method (IEdmState5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html) : GetNextTransition Method (IEdmState5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPosition*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next transition to or from this workflow state (see **Remarks**)

Gets the next transition to or from this workflow state.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextTransition( _    ByVal poPosition As IEdmPos5 _ ) As IEdmTransition5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmTransition5 GetNextTransition(     IEdmPos5 poPosition ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmTransition5^ GetNextTransition(  &   IEdmPos5^ poPosition ) ``` | |

#### Parameters

*poPosition*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next transition to or from this workflow state (see **Remarks**)

#### Return Value

[IEdmTransition5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5.html)

# ![](dotnetimages/collapse.gif)Example

[Get File's State Transitions (C#)](Get_Files_State_Transitions_Example_CSharp.htm)

[Get File's State Transitions (VB.NET)](Get_Files_State_Transitions_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPosition with the interface to the position of the first transition to this workflow state, IEdmPos5. Call [IEdmState5::GetFirstTransitionPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~GetFirstTransitionPosition.html) to start an enumeration and obtain [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html), the position of the first transition.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the transitions to this workflow state.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

C++ programmers must free the interface returned, IEdmFile5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html)

[IEdmState5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2