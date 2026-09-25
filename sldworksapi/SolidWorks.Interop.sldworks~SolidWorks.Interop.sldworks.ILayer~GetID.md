<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer~GetID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetID Method (ILayer) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILayer Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer.html) : GetID Method (ILayer) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the layer ID for this layer.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetID() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILayer Dim value As System.Integer   value = instance.GetID() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetID() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetID(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Layer ID for this layer

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Layer::GetID.

# ![](dotnetimages/collapse.gif)Example

[Get Layers (C#)](Get_Layers_Example_CSharp.htm)

[Get Layers (VB.NET)](Get_Layers_Example_VBNET.htm)

[Get Layers (VBA)](Get_Layers_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

A layer ID:

* is unique within the drawing.* is persistent across SOLIDWORKS sessions and never changes, even if you [change the name of the layer](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer~Name.html).* can be used to identify a specific layer when multiple layers exist in a drawing.* cannot be assigned by applications or users.* is not the same as a persistent reference ID. You can get a layer using its persistent reference ID, but you cannot get a layer using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ILayer Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer.html)

[ILayer Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0