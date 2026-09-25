<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout.html -->

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

| EdmBomLayout Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBomLayout Structure |

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
| ``` Public Structure EdmBomLayout     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmBomLayout : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmBomLayout : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmBomLayout{
  integer [mlLayoutID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout~mlLayoutID.html);
  string [mbsLayoutName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout~mbsLayoutName.html);
};

# ![](dotnetimages/collapse.gif)Example

[Access Bill of Materials (VB.NET)](Access_Bill_of_Materials_Example_VBNET.htm)

[Access Bill of Materials (C#)](Access_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmBomMgr::GetBomLayouts](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr~GetBomLayouts.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmBomLayout Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009