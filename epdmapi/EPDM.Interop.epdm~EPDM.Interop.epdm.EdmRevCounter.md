<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevCounter.html -->

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

| EdmRevCounter Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevCounter_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRevCounter Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Used in calls to [IEdmRevisionMgr::SetRevisionCounters](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~SetRevisionCounters.html), this structure holds information about a single counter.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmRevCounter     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmRevCounter : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmRevCounter : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmRevCounter{
  string [mbsComponentName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevCounter~mbsComponentName.html);
  integer [mlCounter](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevCounter~mlCounter.html);
};

# ![](dotnetimages/collapse.gif)Example

[Set Initial Revision (VB.NET)](Set_Initial_Revision_Example_VBNET.htm)

[Set Initial Revision (C#)](Set_Initial_Revision_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmRevCounter Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevCounter_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007