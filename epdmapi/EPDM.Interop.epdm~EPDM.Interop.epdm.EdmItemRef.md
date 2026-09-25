<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html -->

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

| EdmItemRef Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmItemRef Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about an item reference.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmItemRef     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmItemRef : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmItemRef : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmItemRef

{
  integer [mlEdmRefFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef~mlEdmRefFlags.html);
  string [mbsConfiguration](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef~mbsConfiguration.html);
  object [moNamePathOrID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef~moNamePathOrID.html);
  object [moParentNamePathOrItemID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef~moParentNamePathOrItemID.html);
  integer [mhResult](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef~mhResult.html);
};

# ![](dotnetimages/collapse.gif)Example

[Batch Add Item References (VB.NET)](Batch_Add_and_Remove_Item_References_Example_VBNET.htm)

[Batch Add Item References (C#)](Batch_Add_and_Remove_Item_References_Example_CSharp.htm)

[Get and Set Item References (VB.NET)](Get_and_Set_Item_References_Example_VBNET.htm)

[Get and Set Item References (C#)](Get_and_Set_Item_References_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Used by [IEdmItem::GetReferences](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem~GetReferences.html), [IEdmItem::UpdateReferences](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem~UpdateReferences.html), and [IEdmBatchItemReferenceUpdate::UpdateReferences](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemReferenceUpdate~UpdateReferences.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmItemRef Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010