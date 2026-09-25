<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~LayerName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| LayerName Property (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : LayerName Property (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LayerIndex*
:   Number of the layer whose name to get (see Remarks)

Gets the name of the specified layer in this eDrawings document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property LayerName( _    ByVal LayerIndex As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim LayerIndex As System.Integer Dim value As System.String   value = instance.LayerName(LayerIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.string LayerName(     System.int LayerIndex ) {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ LayerName {    System.String^ get(System.int LayerIndex); } ``` | |

#### Parameters

*LayerIndex*
:   Number of the layer whose name to get (see Remarks)

#### Property Value

Name of specified layer

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::LayerName.

# ![](dotnetimages/collapse.gif)Example

See [IEModelViewControl](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this property, call [IEModelViewControl::LayerCount](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~LayerCount.html) to get the total number of layers in this eDrawings document.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

[IEModelViewControl::ShowLayer Property](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ShowLayer.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2007 SP0