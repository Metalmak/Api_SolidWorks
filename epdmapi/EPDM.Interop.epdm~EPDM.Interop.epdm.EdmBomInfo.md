<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInfo.html -->

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

| EdmBomInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBomInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a Bill of Materials.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmBomInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmBomInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmBomInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmBomInfo{
  integer [mlBomID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInfo~mlBomID.html);
   [enum EdmBomType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInfo~meType.html);
  string [mbsBomName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInfo~mbsBomName.html);
};

# ![](dotnetimages/collapse.gif)Example

[Access Bill of Materials (VB.NET)](Access_Bill_of_Materials_Example_VBNET.htm)

[Access Bill of Materials (C#)](Access_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmFile7::GetDerivedBOMs](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7~GetDerivedBOMs.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmBomInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009