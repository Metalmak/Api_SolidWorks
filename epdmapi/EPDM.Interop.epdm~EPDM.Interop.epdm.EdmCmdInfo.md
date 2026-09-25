<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo.html -->

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

| EdmCmdInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCmdInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about menu command items.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmCmdInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmCmdInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmCmdInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmCmdInfo{
  integer [mlCmdID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo~mlCmdID.html);
  string [mbsCmdStr](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo~mbsCmdStr.html);
  string [mbsTooltip](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo~mbsTooltip.html);
  string [mbsStatusBarHelp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo~mbsStatusBarHelp.html);
  integer [mlEdmMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo~mlEdmMenuFlags.html);
  object [moData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo~moData.html);
};

# ![](dotnetimages/collapse.gif)Example

[Get Menu Command Items (VB.NET)](Get_Menu_Command_Items_Example_VBNET.htm)

[Get Menu Command Items (C#)](Get_Menu_Command_Items_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Used in [IEdmMenu6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu6.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmCmdInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009