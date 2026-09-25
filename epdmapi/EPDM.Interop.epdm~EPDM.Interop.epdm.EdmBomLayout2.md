<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout2.html -->

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

| EdmBomLayout2 Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout2_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBomLayout2 Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a Bill of Materials layout.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmBomLayout2     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmBomLayout2 : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmBomLayout2 : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmBomLayout2{
  integer [mlLayoutID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout~mlLayoutID.html);
  [EdmBomType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout2~meType.html);
  string [mbsLayoutName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout~mbsLayoutName.html);
};

# ![](dotnetimages/collapse.gif)Remarks

This structure:

* Extends [EdmBomLayout](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout.html).* Is used in [IEdmBomMgr2::GetBomLayouts2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2~GetBomLayouts2.html) to get all BOM layouts and BOM types.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmBomLayout2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout2_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2020