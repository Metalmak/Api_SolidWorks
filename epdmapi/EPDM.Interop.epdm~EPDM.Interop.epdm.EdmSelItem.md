<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem.html -->

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

| EdmSelItem Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmSelItem Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about one selected file; e.g., used with [IEdmBatchUnlock::AddSelection](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~AddSelection.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmSelItem     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmSelItem : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmSelItem : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmSelItem

{
  integer [mlDocID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem~mlDocID.html);
  integer [mlProjID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem~mlProjID.html);
};

# ![](dotnetimages/collapse.gif)Example

[Batch Check Out Files (VB.NET)](Batch_Get_Files_Example_VBNET.htm)

[Batch Check Out Files (C#)](Batch_Get_Files_Example_CSharp.htm)

[Access Check-in Flags in Check out Dialog (C#)](Access_Check-in_Flags_in_Check_in_Dialog_Example_CSharp.htm)

[Access Check-in Flags in Check out Dialog (VB.NET)](Access_Check-in_Flags_in_Check_in_Dialog_Example_VBNET.htm)

[Prevent Admin from Checking In File (C#)](Prevent_Admin_from_Checking_In_File_Example_CSharp.htm)

[Prevent Admin from Checking In File (VB.NET)](Prevent_Admin_from_Checking_In_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmSelItem Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional