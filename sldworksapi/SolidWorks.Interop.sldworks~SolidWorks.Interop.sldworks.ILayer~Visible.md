<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer~Visible.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Visible Property (ILayer) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILayer Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer.html) : Visible Property (ILayer) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the visibility of this layer.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Visible As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILayer Dim value As System.Boolean   instance.Visible = value   value = instance.Visible ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Visible {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool Visible {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True if the layer is visible, false if the layer is not visible (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Layer::Visible.

# ![](dotnetimages/collapse.gif)Example

[Determine if Layer is Visible (VBA)](Determine_if_Layer_is_Visible_Example_VB.htm)

[Get Layers (C#)](Get_Layers_Example_CSharp.htm)

[Get Layers (VB.NET)](Get_Layers_Example_VBNET.htm)

[Get Layers (VBA)](Get_Layers_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

After setting this property to the opposite state, call [ILayer::Printable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer~Printable.html) to check its state, because setting ILayer::Visible might change the state of ILayer::Printable.

To ensure that ILayer::Visible and ILayer::Printable are set to the desired states, perform the following steps in this order:

1. Set ILayer::Visible.- Get the state of ILayer::Printable.- Set ILayer::Printable if necessary.

# ![](dotnetimages/collapse.gif)See Also

####

[ILayer Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer.html)

[ILayer Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99 SP6, datecode 1999355