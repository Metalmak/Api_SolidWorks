<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject.html -->

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

| EdmSelectionObject Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmSelectionObject Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains data returned from [IEdmSelectionList6::GetNext2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6~GetNext2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmSelectionObject     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmSelectionObject : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmSelectionObject : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmSelectionObject{
  [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject~meType.html);
  string [mbsPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject~mbsPath.html);
  integer [mlID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject~mlID.html);
  integer [mlProjectID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject~mlProjectID.html);
  integer [mlGetVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject~mlGetVersion.html);
  integer [mlLocalVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject~mlLocalVersion.html);
  integer [mlLatestVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject~mlLatestVersion.html);
};

# ![](dotnetimages/collapse.gif)Example

[Batch Change States of Files (VB.NET)](Batch_Change_States_of_Files_Example_VBNET.htm)

[Batch Change States of Files (C#)](Batch_Change_States_of_Files_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmSelectionObject Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010