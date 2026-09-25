<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError2.html -->

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

| EdmBatchError2 Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError2_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBatchError2 Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains error information.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmBatchError2     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmBatchError2 : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmBatchError2 : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmBatchError2{
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError2~mlFileID.html);
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError2~mlFolderID.html);
  integer [mlVariableID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError2~mlVariableID.html);
  integer [mlErrorCode](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError2~mlErrorCode.html);
};

# ![](dotnetimages/collapse.gif)Example

[Batch Update Card Variables (VB.NET)](Batch_Update_Variables_Example_VBNET.htm)

[Batch Update Card Variables (C#)](Batch_Update_Variables_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Extends the [EdmBatchError structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError.html) and is returned by [IEdmBatchUpdate2::CommitUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~CommitUpdate.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmBatchError2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError2_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional