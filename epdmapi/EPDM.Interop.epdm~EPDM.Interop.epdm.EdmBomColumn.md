<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn.html -->

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

| EdmBomColumn Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBomColumn Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a single column in a Bill of Materials.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmBomColumn     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmBomColumn : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmBomColumn : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmBomColumn{
  integer [mlColumnID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn~mlColumnID.html);
  integer [mlVariableID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn~mlVariableID.html);
  [enum EdmVariableType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableType.html) [mlVariableType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn~mlVariableType.html);
  integer [mlFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn~mlFlags.html);
  [enum EdmBomColumnType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumnType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn~meType.html);
  string [mbsCaption](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn~mbsCaption.html);
  integer [mlWidth](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn~mlWidth.html);
};

# ![](dotnetimages/collapse.gif)Example

[Access Bill of Materials (VB.NET)](Access_Bill_of_Materials_Example_VBNET.htm)

[Access Bill of Materials (C#)](Access_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmBomColumn Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009