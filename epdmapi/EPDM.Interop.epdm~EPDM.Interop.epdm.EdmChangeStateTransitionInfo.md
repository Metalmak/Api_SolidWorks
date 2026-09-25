<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo.html -->

![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/drpdown.gif)
![](dotnetimages/drpdown_orange.gif)
![](dotnetimages/copycode.gif)
![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |

| EdmChangeStateTransitionInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmChangeStateTransitionInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Workflow state transition information.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmChangeStateTransitionInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmChangeStateTransitionInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmChangeStateTransitionInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmChangeStateTransitionInfo

{
  short [mbIsRevoke](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo~mbIsRevoke.html);
  integer [mlCommitsNum](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo~mlCommitsNum.html);
  integer [mlRequiredNum](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo~mlRequiredNum.html);
  string [moDescription](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo~moDescription.html);
  string [moIcon](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo~moIcon.html);
  string [moName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo~moName.html);
 };

# ![](dotnetimages/collapse.gif)Example

[Batch Change States of Files (VB.NET)](Batch_Change_States_of_Files_Example_VBNET.htm)

[Batch Change States of Files (C#)](Batch_Change_States_of_Files_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmChangeStateTransitionInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateTransitionInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013