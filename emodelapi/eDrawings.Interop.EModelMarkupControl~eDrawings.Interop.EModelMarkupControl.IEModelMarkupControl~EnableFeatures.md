<!-- source: emodelapi/eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~EnableFeatures.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| EnableFeatures Property (IEModelMarkupControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelMarkupControl Namespace](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl_namespace.html) > [IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html) : EnableFeatures Property (IEModelMarkupControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets markup properties of the [IEModelMarkupControl](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EnableFeatures As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelMarkupControl Dim value As System.Integer   instance.EnableFeatures = value   value = instance.EnableFeatures ``` | |

| C# |  |
| --- | --- |
| ``` System.int EnableFeatures {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int EnableFeatures {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Value of the bitmask as defined by [EMVMarkupEnableFeatures](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.EMVMarkupEnableFeatures.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelMarkupControl::EnableFeatures.

# ![](dotnetimages/collapse.gif)Remarks

You can only set this property at runtime; you cannot set it at design time.

To set an individual markup property only, use [IEModelMarkupControl::EnableFeature](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~EnableFeature.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html)

[IEModelMarkupControl Members](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0