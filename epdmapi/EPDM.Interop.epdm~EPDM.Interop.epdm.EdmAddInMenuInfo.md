<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo.html -->

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

| EdmAddInMenuInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmAddInMenuInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a menu command implemented by an add-in.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmAddInMenuInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmAddInMenuInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmAddInMenuInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmAddInMenuInfo{
  integer  [mlCmdID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo~mlCmdID.html);
  integer  [mlEdmMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo~mlEdmMenuFlags.html);
  integer  [mlToolbarButtonIndex](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo~mlToolbarButtonIndex.html);
  integer  [mlToolbarImageID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo~mlToolbarImageID.html);
  string  [mbsMenuStr](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo~mbsMenuStr.html);
  string  [mbsStatusBarHelp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo~mbsStatusBarHelp.html);
  string  [mbsToolbarToolTip](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo~mbsToolbarToolTip.html);
};

# ![](dotnetimages/collapse.gif)Example

[Install Add-in (VB.NET)](Load_Addin_Example_VBNET.htm)

[Install Add-in (C#)](Load_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmAddInMgr8::GetInstalledAddIn](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8~GetInstalledAddIn.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmAddInMenuInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010