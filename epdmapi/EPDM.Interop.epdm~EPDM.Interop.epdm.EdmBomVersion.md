<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion.html -->

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

| EdmBomVersion Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBomVersion Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a Bill of Materials version, revision, or label.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmBomVersion     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmBomVersion : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmBomVersion : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmBomVersion{
  [enum EdmBomVersionType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersionType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion~meType.html);
  integer [mlVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion~mlVersion.html);
  datetime [moDate](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion~moDate.html);
  string [mbsTag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion~mbsTag.html);
  string [mbsComment](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion~mbsComment.html);
};

# ![](dotnetimages/collapse.gif)Example

[Access Bill of Materials (VB.NET)](Access_Bill_of_Materials_Example_VBNET.htm)

[Access Bill of Materials (C#)](Access_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmBomVersion Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009