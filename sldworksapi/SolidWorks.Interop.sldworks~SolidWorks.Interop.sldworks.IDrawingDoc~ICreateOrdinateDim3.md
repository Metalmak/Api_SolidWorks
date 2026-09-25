<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateOrdinateDim3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateOrdinateDim3 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateOrdinateDim3 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*P0*

*P1*

*P2*

*P3*

*P4*

*Angle*

*ArrowSize*

*Text*

*TextHeight*

*WitnessGap*

*WitnessOvershoot*

*P5*

Obsolete. Superseded by [IDrawingDoc::ICreateOrdinateDim4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateOrdinateDim4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateOrdinateDim3( _    ByRef P0 As System.Double, _    ByRef P1 As System.Double, _    ByRef P2 As System.Double, _    ByRef P3 As System.Double, _    ByRef P4 As System.Double, _    ByVal Angle As System.Double, _    ByVal ArrowSize As System.Double, _    ByVal Text As System.String, _    ByVal TextHeight As System.Double, _    ByVal WitnessGap As System.Double, _    ByVal WitnessOvershoot As System.Double, _    ByRef P5 As System.Double _ ) As DisplayDimension ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim P0 As System.Double Dim P1 As System.Double Dim P2 As System.Double Dim P3 As System.Double Dim P4 As System.Double Dim Angle As System.Double Dim ArrowSize As System.Double Dim Text As System.String Dim TextHeight As System.Double Dim WitnessGap As System.Double Dim WitnessOvershoot As System.Double Dim P5 As System.Double Dim value As DisplayDimension   value = instance.ICreateOrdinateDim3(P0, P1, P2, P3, P4, Angle, ArrowSize, Text, TextHeight, WitnessGap, WitnessOvershoot, P5) ``` | |

| C# |  |
| --- | --- |
| ``` DisplayDimension ICreateOrdinateDim3(     ref System.double P0,    ref System.double P1,    ref System.double P2,    ref System.double P3,    ref System.double P4,    System.double Angle,    System.double ArrowSize,    System.string Text,    System.double TextHeight,    System.double WitnessGap,    System.double WitnessOvershoot,    ref System.double P5 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` DisplayDimension^ ICreateOrdinateDim3(  &   System.double% P0, &   System.double% P1, &   System.double% P2, &   System.double% P3, &   System.double% P4, &   System.double Angle, &   System.double ArrowSize, &   System.String^ Text, &   System.double TextHeight, &   System.double WitnessGap, &   System.double WitnessOvershoot, &   System.double% P5 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*P0*

*P1*

*P2*

*P3*

*P4*

*Angle*

*ArrowSize*

*Text*

*TextHeight*

*WitnessGap*

*WitnessOvershoot*

*P5*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateOrdinateDim3.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)