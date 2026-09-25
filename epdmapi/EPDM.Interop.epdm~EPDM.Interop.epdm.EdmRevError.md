<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevError.html -->

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

| EdmRevError Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevError_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRevError Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Returned from [IEdmRevisionMgr::Commit](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~Commit.html) if something goes wrong when incrementing the revision number on a file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmRevError     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmRevError : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmRevError : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmRevError{
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevError~mlFileID.html);
  integer [mhError](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevError~mhError.html);
};

# ![](dotnetimages/collapse.gif)Example

[Set Initial Revision (VB.NET)](Set_Initial_Revision_Example_VBNET.htm)

[Set Initial Revision (C#)](Set_Initial_Revision_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmRevError Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevError_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007