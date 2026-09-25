<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr~AddLayer.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddLayer Method (ILayerMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILayerMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr.html) : AddLayer Method (ILayerMgr) |

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

*DescIn*
:   Description for the new layer

*ColorIn*
:   COLORREF value specifying the desired color of items within this layer

*StyleIn*
:   Line style as defined in swLineStyles\_e

*WidthIn*
:   Line width as defined in swLineWeights\_e

Adds a layer to this drawing document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddLayer( _    ByVal NameIn As System.String, _    ByVal DescIn As System.String, _    ByVal ColorIn As System.Integer, _    ByVal StyleIn As System.Integer, _    ByVal WidthIn As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILayerMgr Dim NameIn As System.String Dim DescIn As System.String Dim ColorIn As System.Integer Dim StyleIn As System.Integer Dim WidthIn As System.Integer Dim value As System.Integer   value = instance.AddLayer(NameIn, DescIn, ColorIn, StyleIn, WidthIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddLayer(     System.string NameIn,    System.string DescIn,    System.int ColorIn,    System.int StyleIn,    System.int WidthIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddLayer(  &   System.String^ NameIn, &   System.String^ DescIn, &   System.int ColorIn, &   System.int StyleIn, &   System.int WidthIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NameIn*
:   Layer name

*DescIn*
:   Description for the new layer

*ColorIn*
:   COLORREF value specifying the desired color of items within this layer

*StyleIn*
:   Line style as defined in swLineStyles\_e

*WidthIn*
:   Line width as defined in swLineWeights\_e

#### Return Value

1 if the layer was created successfully

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LayerMgr::AddLayer.

# ![](dotnetimages/collapse.gif)See Also

####

[ILayerMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr.html)

[ILayerMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207