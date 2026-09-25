<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2.html -->

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

| EdmRevComponent2 Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRevComponent2 Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Holds information about a single revision number component.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmRevComponent2     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmRevComponent2 : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmRevComponent2 : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmRevComponent2{
  integer [mlComponentID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mlComponentID.html);
  string [mbsComponentName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mbsComponentName.html);
  integer [mlEdmRevComponentFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mlEdmRevComponentFlags.html);
  string [mbsData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mbsData.html);
  integer [mlRecipientID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mlRecipientID.html);
  integer [mlInitialCounter](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mlInitialCounter.html);
};

# ![](dotnetimages/collapse.gif)Example

[Find Revisions Using Component (C#)](Find_Revisions_Using_Component_Example_CSharp.htm)

[Find Revisions Using Component (VB.NET)](Find_Revisions_Using_Component_Example_VBNET.htm)

[Set Initial Revision (VB.NET)](Set_Initial_Revision_Example_VBNET.htm)

[Set Initial Revision (C#)](Set_Initial_Revision_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can obtain this structure by calling [IEdmRevisionMgr2::GetRevisionNumberComponents2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2~GetRevisionNumberComponents2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmRevComponent2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007 SP03