<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent.html -->

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

| EdmRevComponent Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRevComponent Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [EdmRevComponent2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmRevComponent     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmRevComponent : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmRevComponent : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmRevComponent

{
  integer [mlComponentID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent~mlComponentID.html);
  string [mbsComponentName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent~mbsComponentName.html);
};

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmRevisionMgr::GetRevisionNumberComponents](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~GetRevisionNumberComponents.html), which is obsolete and superseded by [IEdmRevisionMgr2.::GetRevisionNumberComponents2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2~GetRevisionNumberComponents2.html), which returns EdmRevComponent2.

The struct contains the component information.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmRevComponent Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007