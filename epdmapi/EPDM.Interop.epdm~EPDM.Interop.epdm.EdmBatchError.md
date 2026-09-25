<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError.html -->

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

| EdmBatchError Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBatchError Structure |

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
| ``` Public Structure EdmBatchError     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmBatchError : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmBatchError : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmBatchError{
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError~mlFileID.html);
  integer [mlVariableID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError~mlVariableID.html);
  integer [mlErrorCode](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError~mlErrorCode.html);
};

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmBatchUpdate::Commit](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate~Commit.html)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmBatchError Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.2 of SOLIDWORKS PDM Professional