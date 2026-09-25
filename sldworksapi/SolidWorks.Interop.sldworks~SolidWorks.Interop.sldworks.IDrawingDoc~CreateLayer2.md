<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateLayer2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateLayer2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateLayer2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Layername*
:   Layer name (see **Remarks**)

*LayerDesc*
:   Description for the new layer

*LayerColor*
:   COLORREF value specifying the color of items in this layer

*LayerStyle*
:   Line style as defined in swLineStyles\_e

*LayerWidth*
:   Line width as defined in swLineWeights\_e

*BOn*
:   True makes this layer visible, false makes it invisible

*BPrint*
:   True to print this layer when printing the document, false to not

Creates a layer for this document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateLayer2( _    ByVal Layername As System.String, _    ByVal LayerDesc As System.String, _    ByVal LayerColor As System.Integer, _    ByVal LayerStyle As System.Integer, _    ByVal LayerWidth As System.Integer, _    ByVal BOn As System.Boolean, _    ByVal BPrint As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Layername As System.String Dim LayerDesc As System.String Dim LayerColor As System.Integer Dim LayerStyle As System.Integer Dim LayerWidth As System.Integer Dim BOn As System.Boolean Dim BPrint As System.Boolean Dim value As System.Boolean   value = instance.CreateLayer2(Layername, LayerDesc, LayerColor, LayerStyle, LayerWidth, BOn, BPrint) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateLayer2(     System.string Layername,    System.string LayerDesc,    System.int LayerColor,    System.int LayerStyle,    System.int LayerWidth,    System.bool BOn,    System.bool BPrint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateLayer2(  &   System.String^ Layername, &   System.String^ LayerDesc, &   System.int LayerColor, &   System.int LayerStyle, &   System.int LayerWidth, &   System.bool BOn, &   System.bool BPrint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Layername*
:   Layer name (see **Remarks**)

*LayerDesc*
:   Description for the new layer

*LayerColor*
:   COLORREF value specifying the color of items in this layer

*LayerStyle*
:   Line style as defined in swLineStyles\_e

*LayerWidth*
:   Line width as defined in swLineWeights\_e

*BOn*
:   True makes this layer visible, false makes it invisible

*BPrint*
:   True to print this layer when printing the document, false to not

#### Return Value

True if the layer was created successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateLayer2.

# ![](dotnetimages/collapse.gif)Example

[Create Layer for Selected View (VBA)](Create_Layer_for_Selected_View_Example_VB.htm)

[Create Layer for Selected View (VB.NET)](Create_Layer_for_Selected_View_Example_VBNET.htm)

[Create Layer for Selected View (C#)](Create_Layer_for_Selected_View_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If this layer is not visible, then SOLIDWORKS does not display entities on the layer.

Do not use backslash or @ symbols in Layername.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::SetCurrentLayer Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~SetCurrentLayer.html)

[ILayer Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer.html)

[ILayerMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayerMgr.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0