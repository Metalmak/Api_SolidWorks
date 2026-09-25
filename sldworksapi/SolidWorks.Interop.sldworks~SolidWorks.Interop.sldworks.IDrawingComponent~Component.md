<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent~Component.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Component Property (IDrawingComponent) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingComponent Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent.html) : Component Property (IDrawingComponent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the assembly component referenced in this drawing component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property Component As Component2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingComponent Dim value As Component2   value = instance.Component ``` | |

| C# |  |
| --- | --- |
| ``` Component2 Component {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property Component2^ Component {    Component2^ get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Associated [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) object for the referenced assembly document

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingComponent::Component.

# ![](dotnetimages/collapse.gif)Example

[Get Components in Drawing View (VBA)](Get_Components_in_Drawing_View_Example_VB.htm)

[Get Components in Drawing View (VB.NET)](Get_Components_in_Drawing_View_Example_VBNET.htm)

[Get Components in Drawing View (C#)](Get_Components_in_Drawing_View_Example_CSharp.htm)

[Select Drawing Component (C#)](Select_Drawing_Component_Example_CSharp.htm)

[Select Drawing Component (VB.NET)](Select_Drawing_Component_Example_VBNET.htm)

[Select Drawing Component (VBA)](Select_Drawing_Component_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The associated [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) object should have the same properties as the referenced configuration. For example, if the component is suppressed in the reference configuration, then the returned component should also be suppressed.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingComponent Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent.html)

[IDrawingComponent Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0