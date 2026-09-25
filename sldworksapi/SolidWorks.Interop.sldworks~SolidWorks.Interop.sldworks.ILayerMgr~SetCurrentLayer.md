<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr~SetCurrentLayer.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetCurrentLayer Method (ILayerMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILayerMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr.html) : SetCurrentLayer Method (ILayerMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NameIn*
:   Name of the layer to become the active layer

Sets the current (or active) layer in this drawing document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetCurrentLayer( _    ByVal NameIn As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILayerMgr Dim NameIn As System.String Dim value As System.Integer   value = instance.SetCurrentLayer(NameIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetCurrentLayer(     System.string NameIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetCurrentLayer(  &   System.String^ NameIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NameIn*
:   Name of the layer to become the active layer

#### Return Value

1 if the active layer was changed to the specified layer, 0 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LayerMgr::SetCurrentLayer.

# ![](dotnetimages/collapse.gif)See Also

####

[ILayerMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr.html)

[ILayerMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr_members.html)

[ILayerMgr::GetCurrentLayer Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr~GetCurrentLayer.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207