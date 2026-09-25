<!-- source: emodelapi/eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~EnableFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| EnableFeature Property (IEModelMarkupControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelMarkupControl Namespace](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl_namespace.html) > [IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html) : EnableFeature Property (IEModelMarkupControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*feature*
:   Markup property as defined in [EMVMarkupEnableFeatures](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.EMVMarkupEnableFeatures.html)

Gets or sets the specified markup property.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EnableFeature( _    ByVal feature As EMVMarkupEnableFeatures _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelMarkupControl Dim feature As EMVMarkupEnableFeatures Dim value As System.Boolean   instance.EnableFeature(feature) = value   value = instance.EnableFeature(feature) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EnableFeature(     EMVMarkupEnableFeatures feature ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool EnableFeature {    System.bool get(EMVMarkupEnableFeatures feature);    void set (EMVMarkupEnableFeatures feature, System.bool value); } ``` | |

#### Parameters

*feature*
:   Markup property as defined in [EMVMarkupEnableFeatures](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.EMVMarkupEnableFeatures.html)

#### Property Value

True if the markup property is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelMarkupControl::EnableFeature.

# ![](dotnetimages/collapse.gif)Remarks

You can only set this property at runtime; you cannot set it at design time.

To set multiple markup properties at the same time, use [IEModelMarkupViewControl::EnableFeatures](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~EnableFeatures.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html)

[IEModelMarkupControl Members](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0