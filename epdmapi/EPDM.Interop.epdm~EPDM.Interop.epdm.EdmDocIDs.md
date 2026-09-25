<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDocIDs.html -->

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

| EdmDocIDs Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDocIDs_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmDocIDs Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about one document in the vault; used in [IEdmVault20::GetFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20~GetFiles.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmDocIDs     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmDocIDs : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmDocIDs : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmDocIDs

{
  integer [mlDocID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDocIDs~mlDocID.html);
  integer [mlProjID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDocIDs~mlProjID.html);
};

# ![](dotnetimages/collapse.gif)See Also

####

[EdmDocIDs Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDocIDs_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)