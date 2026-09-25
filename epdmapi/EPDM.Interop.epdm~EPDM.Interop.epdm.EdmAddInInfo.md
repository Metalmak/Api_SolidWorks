<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo.html -->

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

| EdmAddInInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmAddInInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Provides SOLIDWORKS PDM Professional with information about your add-in.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmAddInInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmAddInInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmAddInInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmAddInInfo{
  string [mbsAddInName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo~mbsAddInName.html);
  string [mbsCompany](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo~mbsCompany.html);
  string [mbsDescription](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo~mbsDescription.html);
  integer [mlAddInVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo~mlAddInVersion.html);
  integer [mlRequiredVersionMajor](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo~mlRequiredVersionMajor.html);
  integer [mlRequiredVersionMinor](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo~mlRequiredVersionMinor.html);
};

# ![](dotnetimages/collapse.gif)Example

[Notify User When File Changes State (VB.NET)](Notify_User_When_File_Changes_State_Example_VBNET.htm)

[Notify User When File Changes State (C#)](Notify_User_When_File_Changes_State_Example_CSharp.htm)

[Create a Task that Finds Approved Files (VB.NET)](Schedule_Task_Addin_Example_VBNET.htm)

[Create a Task that Finds Approved Files (C#)](Schedule_Task_Addin_Example_CSharp.htm)

[Change Card Variables Add-in (VB.NET)](Change_Card_Variables_Addin_Example_VBNET.htm)

[Change Card Variables Add-in (C#)](Change_Card_Variables_Addin_Example_CSharp.htm)

[Create a Task that Finds Files in Workflow States (VB.NET)](Schedule_Task_to_Find_Files_in_State_Addin_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (C#))](Schedule_Task_to_Find_Files_in_State_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html).

The data is displayed in the [Administrate Add-ins dialog box](AdminDlg.htm). If your add-in relies on features in a specific version of SOLIDWORKS PDM Professional, make it impossible to load the add-in in older versions of SOLIDWORKS PDM Professional by populating the mlRequiredVersionMajor and mlRequiredVersionMinor members.

C++ programmers must set string members to strings allocated with the Win32 function SysAllocString.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmAddInInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional