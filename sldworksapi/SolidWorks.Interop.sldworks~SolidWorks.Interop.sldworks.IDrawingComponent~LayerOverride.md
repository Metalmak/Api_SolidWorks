<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent~LayerOverride.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LayerOverride Property (IDrawingComponent) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingComponent Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent.html) : LayerOverride Property (IDrawingComponent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether the drawing component has properties that override the default properties of the layer.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property LayerOverride As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingComponent Dim value As System.Integer   instance.LayerOverride = value   value = instance.LayerOverride ``` | |

| C# |  |
| --- | --- |
| ``` System.int LayerOverride {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int LayerOverride {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Properties that have been overridden or should be overridden as defined in  swLayerOverride\_e (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingComponent::LayerOverride.

# ![](dotnetimages/collapse.gif)Example

[Get Components' Properties in Drawing View (VBA)](Get_Components_Properties_in_Drawing_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Currently, only SOLIDWORKS drawing documents support layers.

You should set this property only when you want to reset specific visual properties to the default visual properties of the owning layer. If you want to change or set specific values for the visual property of this component, use [IDrawingComponent::Style](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingComponent~Style.html) or [IDrawingComponent::Width](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingComponent~Width.html).

In drawing documents, components can be created on a layer that has specific visual properties. By default, the component takes on the visual properties defined by the layer. However, for a specific component, you can override these visual properties (style or width).

When the component is not on any layer, this property returns an undefined value. You can use [IDrawingComponent::Layer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingComponent~Layer.html) to determine the name of the layer that this component is on. If an empty string is returned by this property, then this property is not used.

When you get this property, the returned bit value indicates which properties have been overridden. The bit indicators are:

* color = 0x1

  * style = 0x2

    * width = 0x4

Therefore, if the return value is returned as 2, then you know style has been specifically set for this component and might not match the default value associated with this component's layer.

When you set this property, the input bit value indicates which properties should maintain their current override values. Therefore, if the return value is passed as 0x4, you know width should keep its current override value and style should be reset to use the style settings for the component's layer. If you pass 0, all visual properties are reset to use the default settings of the component's layer.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingComponent Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent.html)

[IDrawingComponent Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0