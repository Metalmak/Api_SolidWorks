<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint~LayerOverride.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LayerOverride Property (ISketchPoint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchPoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html) : LayerOverride Property (ISketchPoint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether the sketch point has properties that override the default properties of the layer.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property LayerOverride As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchPoint Dim value As System.Integer   instance.LayerOverride = value   value = instance.LayerOverride ``` | |

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

See SketchPoint::LayerOverride.

# ![](dotnetimages/collapse.gif)Remarks

Layers are supported only in drawing documents.

In drawing documents, sketch points can be created on a layer that has specific visual properties. By default, the sketch point inherits the visual properties defined by the layer. However, for a specific sketch point, these visual properties can be overridden.

When the sketch point is not on any layer, the value this property returns is undefined. You can use the [ISketchPoint::Layer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchPoint~Layer.html) property to determine the name of the layer, if any, that this sketch point is on. If an empty string is returned by the ISketchPoint::Layer property, then this  property is not used.

Sketch points currently support only the color visual property. Therefore, the only bit value that is currently used by this function is 0x1, which indicates a color override. If this property returns 0x1, this indicates that the color of this sketch point has been specifically set by the end-user and may not match the default color value associated with this sketch point's layer. If you pass 0 to this property, then you are indicating that the color should be reset to use the default color associated with this item's layer.

Only set this property to reset specific visual properties back to the default visual properties of the owning layer. If you want to change or set specific values for the visual property for this item, use [ISketchPoint::Color](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchPoint~Color.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html)

[ISketchPoint Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207