<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateDiamDim2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateDiamDim2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateDiamDim2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DimValue*

*P0*

*P1*

*P2*

*P3*

*ArrowSize*

*Text*

*TextHeight*

*WitnessGap*

*WitnessOvershoot*

*TextPoint*

Obsolete. Superseded by [IDrawingDoc::ICreateDiamDim4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~ICreateDiamDim4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ICreateDiamDim2( _    ByVal DimValue As System.Double, _    ByRef P0 As System.Double, _    ByRef P1 As System.Double, _    ByRef P2 As System.Double, _    ByRef P3 As System.Double, _    ByVal ArrowSize As System.Double, _    ByVal Text As System.String, _    ByVal TextHeight As System.Double, _    ByVal WitnessGap As System.Double, _    ByVal WitnessOvershoot As System.Double, _    ByRef TextPoint As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim DimValue As System.Double Dim P0 As System.Double Dim P1 As System.Double Dim P2 As System.Double Dim P3 As System.Double Dim ArrowSize As System.Double Dim Text As System.String Dim TextHeight As System.Double Dim WitnessGap As System.Double Dim WitnessOvershoot As System.Double Dim TextPoint As System.Double   instance.ICreateDiamDim2(DimValue, P0, P1, P2, P3, ArrowSize, Text, TextHeight, WitnessGap, WitnessOvershoot, TextPoint) ``` | |

| C# |  |
| --- | --- |
| ``` void ICreateDiamDim2(     System.double DimValue,    ref System.double P0,    ref System.double P1,    ref System.double P2,    ref System.double P3,    System.double ArrowSize,    System.string Text,    System.double TextHeight,    System.double WitnessGap,    System.double WitnessOvershoot,    ref System.double TextPoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ICreateDiamDim2(  &   System.double DimValue, &   System.double% P0, &   System.double% P1, &   System.double% P2, &   System.double% P3, &   System.double ArrowSize, &   System.String^ Text, &   System.double TextHeight, &   System.double WitnessGap, &   System.double WitnessOvershoot, &   System.double% TextPoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DimValue*

*P0*

*P1*

*P2*

*P3*

*ArrowSize*

*Text*

*TextHeight*

*WitnessGap*

*WitnessOvershoot*

*TextPoint*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateDiamDim2.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)