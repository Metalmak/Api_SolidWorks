<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr~GetLayer.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetLayer Method (ILayerMgr) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILayerMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr.html) : GetLayer Method (ILayerMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NameIn*
:   Layer name

Gets the specified layer in this drawing document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetLayer( _    ByVal NameIn As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILayerMgr Dim NameIn As System.String Dim value As System.Object   value = instance.GetLayer(NameIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetLayer(     System.string NameIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetLayer(  &   System.String^ NameIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NameIn*
:   Layer name

#### Return Value

Layer

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LayerMgr::GetLayer.

# ![](dotnetimages/collapse.gif)Example

[Determine If Layer Is Visible (VBA)](Determine_if_Layer_is_Visible_Example_VB.htm)

[Get Layers (C#)](Get_Layers_Example_CSharp.htm)

[Get Layers (VB.NET)](Get_Layers_Example_VBNET.htm)

[Get Layers (VBA)](Get_Layers_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can get the layer name by calling [ILayerMgr::GetCurrentLayer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILayerMgr~GetCurrentLayer.html), create a new layer calling [ILayerMgr::AddLayer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILayerMgr~AddLayer.html), or obtain a list of layer names by calling [ILayerMgr::GetLayerList](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILayerMgr~GetLayerList.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ILayerMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr.html)

[ILayerMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr_members.html)

[ILayerMgr::IGetLayer Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr~IGetLayer.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, Revision Number 1999207