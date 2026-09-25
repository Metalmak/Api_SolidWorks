<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevNo.html -->

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

| EdmRevNo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevNo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRevNo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Holds information about a revision number and is returned from [IEdmRevisionMgr2::GetRevisionNumbers](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2~GetRevisionNumbers.html)..

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmRevNo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmRevNo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmRevNo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmRevNo{
  integer [mlRevNoID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevNo~mlRevNoID.html);
  string [mbsRevNoName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevNo~mbsRevNoName.html);
  string [mbsData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevNo~mbsData.html);
};

# ![](dotnetimages/collapse.gif)Example

[Find Revisions Using Component (C#)](Find_Revisions_Using_Component_Example_CSharp.htm)

[Find Revisions Using Component (VB.NET)](Find_Revisions_Using_Component_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can get the components of a revision number by calling [IEdmRevisionMgr2::GetRevisionNumberComponents2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2~GetRevisionNumberComponents2.html) and passing a negative value to the EdmRevNo struct's [mlRevNoID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevNo~mlRevNoID.html) field as the argument.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmRevNo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevNo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007 SP03