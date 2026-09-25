<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockErrInfo.html -->

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

| EdmUnlockErrInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockErrInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUnlockErrInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains extended information about an error message.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmUnlockErrInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmUnlockErrInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmUnlockErrInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmUnlockErrInfo{
  integer [mlDocID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockErrInfo~mlDocID.html);
  string [mbsConfigName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockErrInfo~mbsConfigName.html);
  integer [mlVarID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockErrInfo~mlVarID.html);
  string [mbsVarName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockErrInfo~mbsVarName.html);
};

# ![](dotnetimages/collapse.gif)Example

[Prevent Admin from Checking In File (C#)](Prevent_Admin_from_Checking_In_File_Example_CSharp.htm)

[Prevent Admin from Checking In File (VB.NET)](Prevent_Admin_from_Checking_In_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This struct is displayed with [IEdmUnlockOpCallback::MsgBox](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~MsgBox.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmUnlockErrInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockErrInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional