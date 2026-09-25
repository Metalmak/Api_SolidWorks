<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmWorkflowInfo.html -->

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

| EdmWorkflowInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmWorkflowInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmWorkflowInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Holds information about a file's workflow state.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmWorkflowInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmWorkflowInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmWorkflowInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmWorkflowInfo
  string [mbsStateName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmWorkflowInfo~mbsStateName.html);
  string [mbsStateIcon](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmWorkflowInfo~mbsStateIcon.html);
  string [mbsWorkflowName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmWorkflowInfo~mbsWorkflowName.html);
};

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This structure is referenced in the [EdmListFile2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2.html) structure.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmWorkflowInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmWorkflowInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional