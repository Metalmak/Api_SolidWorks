<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData.html -->

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

| EdmGetVarData Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGetVarData Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains extra file information.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmGetVarData     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmGetVarData : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmGetVarData : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmGetVarData{
  integer [mlVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData~mlVersion.html);
  integer [mlLatestVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData~mlLatestVersion.html);
  string [mbsRevision](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData~mbsRevision.html);
  string [mbsState](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData~mbsState.html);
  string [mbsWorkflow](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData~mbsWorkflow.html);
  string [mbsCategory](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData~mbsCategory.html);
  integer [mlDateFmt](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData~mlDateFmt.html);
  integer [mlEdmGetVarDataFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData~mlEdmGetVarDataFlags.html);
};

# ![](dotnetimages/collapse.gif)Example

[Get File Variable Data (VB.NET)](Get_File_Variable_Data_Example_VBNET.htm)

[Get File Variable Data (C#)](Get_File_Variable_Data_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmEnumeratorVariable7::GetVersionVars](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7~GetVersionVars.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmGetVarData Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional