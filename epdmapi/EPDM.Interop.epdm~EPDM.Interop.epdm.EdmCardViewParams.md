<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams.html -->

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

| EdmCardViewParams Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCardViewParams Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains card view parameters.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmCardViewParams     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmCardViewParams : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmCardViewParams : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmCardViewParams{
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams~mlFileID.html);
  integer [mlFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams~mlFolderID.html);
  integer [mlCardID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams~mlCardID.html);
  integer [mlX](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams~mlX.html);
  integer [mlY](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams~mlY.html);
  integer [mhParentWindow](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams~mhParentWindow.html);
  integer [mlEdmCardViewFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams~mlEdmCardViewFlags.html);
};

# ![](dotnetimages/collapse.gif)Example

[Create Custom Card View (VB.NET)](Create_Custom_Card_View_Example_VBNET.htm)

[Create Custom Card View (C#)](Create_Custom_Card_View_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Used by [IEdmVault10::CreateCardViewEx2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10~CreateCardViewEx2.html) to create a card view.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmCardViewParams Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewParams_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009