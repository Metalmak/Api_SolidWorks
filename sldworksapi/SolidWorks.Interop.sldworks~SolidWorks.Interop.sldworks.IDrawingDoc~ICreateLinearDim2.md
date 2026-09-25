<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateLinearDim2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateLinearDim2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateLinearDim2 Method (IDrawingDoc) |

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

*Val*

*PrimPrec*

*Text*

*TextPoint*

*Angle*

*TextHeight*

*Prefix*

*Suffix*

*Callout1*

*Callout2*

*TolType*

*TolMin*

*TolMax*

*TolPrec*

*ArrowSize*

*ArrowStyle*

*ArrowDir*

*WitnessGap*

*WitnessOvershoot*

*DualDisplay*

*DualPrecision*

Obsolete. Superseded by [IDrawingDoc::ICreateLinearDim4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateLinearDim4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ICreateLinearDim2( _    ByRef P0 As System.Double, _    ByRef P1 As System.Double, _    ByRef P2 As System.Double, _    ByRef P3 As System.Double, _    ByRef P4 As System.Double, _    ByVal Val As System.Double, _    ByVal PrimPrec As System.Integer, _    ByVal Text As System.String, _    ByRef TextPoint As System.Double, _    ByVal Angle As System.Double, _    ByVal TextHeight As System.Double, _    ByVal Prefix As System.String, _    ByVal Suffix As System.String, _    ByVal Callout1 As System.String, _    ByVal Callout2 As System.String, _    ByVal TolType As System.Integer, _    ByVal TolMin As System.String, _    ByVal TolMax As System.String, _    ByVal TolPrec As System.Integer, _    ByVal ArrowSize As System.Double, _    ByVal ArrowStyle As System.Integer, _    ByVal ArrowDir As System.Integer, _    ByVal WitnessGap As System.Double, _    ByVal WitnessOvershoot As System.Double, _    ByVal DualDisplay As System.Boolean, _    ByVal DualPrecision As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim P0 As System.Double Dim P1 As System.Double Dim P2 As System.Double Dim P3 As System.Double Dim P4 As System.Double Dim Val As System.Double Dim PrimPrec As System.Integer Dim Text As System.String Dim TextPoint As System.Double Dim Angle As System.Double Dim TextHeight As System.Double Dim Prefix As System.String Dim Suffix As System.String Dim Callout1 As System.String Dim Callout2 As System.String Dim TolType As System.Integer Dim TolMin As System.String Dim TolMax As System.String Dim TolPrec As System.Integer Dim ArrowSize As System.Double Dim ArrowStyle As System.Integer Dim ArrowDir As System.Integer Dim WitnessGap As System.Double Dim WitnessOvershoot As System.Double Dim DualDisplay As System.Boolean Dim DualPrecision As System.Integer   instance.ICreateLinearDim2(P0, P1, P2, P3, P4, Val, PrimPrec, Text, TextPoint, Angle, TextHeight, Prefix, Suffix, Callout1, Callout2, TolType, TolMin, TolMax, TolPrec, ArrowSize, ArrowStyle, ArrowDir, WitnessGap, WitnessOvershoot, DualDisplay, DualPrecision) ``` | |

| C# |  |
| --- | --- |
| ``` void ICreateLinearDim2(     ref System.double P0,    ref System.double P1,    ref System.double P2,    ref System.double P3,    ref System.double P4,    System.double Val,    System.int PrimPrec,    System.string Text,    ref System.double TextPoint,    System.double Angle,    System.double TextHeight,    System.string Prefix,    System.string Suffix,    System.string Callout1,    System.string Callout2,    System.int TolType,    System.string TolMin,    System.string TolMax,    System.int TolPrec,    System.double ArrowSize,    System.int ArrowStyle,    System.int ArrowDir,    System.double WitnessGap,    System.double WitnessOvershoot,    System.bool DualDisplay,    System.int DualPrecision ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ICreateLinearDim2(  &   System.double% P0, &   System.double% P1, &   System.double% P2, &   System.double% P3, &   System.double% P4, &   System.double Val, &   System.int PrimPrec, &   System.String^ Text, &   System.double% TextPoint, &   System.double Angle, &   System.double TextHeight, &   System.String^ Prefix, &   System.String^ Suffix, &   System.String^ Callout1, &   System.String^ Callout2, &   System.int TolType, &   System.String^ TolMin, &   System.String^ TolMax, &   System.int TolPrec, &   System.double ArrowSize, &   System.int ArrowStyle, &   System.int ArrowDir, &   System.double WitnessGap, &   System.double WitnessOvershoot, &   System.bool DualDisplay, &   System.int DualPrecision ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*P0*

*P1*

*P2*

*P3*

*P4*

*Val*

*PrimPrec*

*Text*

*TextPoint*

*Angle*

*TextHeight*

*Prefix*

*Suffix*

*Callout1*

*Callout2*

*TolType*

*TolMin*

*TolMax*

*TolPrec*

*ArrowSize*

*ArrowStyle*

*ArrowDir*

*WitnessGap*

*WitnessOvershoot*

*DualDisplay*

*DualPrecision*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateLinearDim2.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)