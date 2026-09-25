<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem~ItemDescriptiveName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ItemDescriptiveName Property (IEdmItem) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem.html) : ItemDescriptiveName Property (IEdmItem) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the descriptive name of this item.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property ItemDescriptiveName As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string ItemDescriptiveName {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ ItemDescriptiveName {    System.String^ get(); } ``` | |

#### Property Value

Descriptive name of this item

# ![](dotnetimages/collapse.gif)Example

See the [IEdmItem](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The descriptive name of an item is based on a variable in its data card.

An item also has an "item ID", which is its file name counterpart, accessible via the [IEdmItem::Name](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem~ItemDescriptiveName.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem.html)

[IEdmItem Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010