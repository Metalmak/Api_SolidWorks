<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateOrdinateDim.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateOrdinateDim Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateOrdinateDim Method (IDrawingDoc) |

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

Obsolete. Superseded by [IDrawingDoc::CreateOrdinateDim4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateOrdinateDim4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateOrdinateDim( _    ByVal P0 As System.Object, _    ByVal P1 As System.Object, _    ByVal P2 As System.Object, _    ByVal P3 As System.Object, _    ByVal P4 As System.Object, _    ByVal Angle As System.Double, _    ByVal ArrowSize As System.Double, _    ByVal Text As System.String, _    ByVal TextHeight As System.Double, _    ByVal WitnessGap As System.Double, _    ByVal WitnessOvershoot As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim P0 As System.Object Dim P1 As System.Object Dim P2 As System.Object Dim P3 As System.Object Dim P4 As System.Object Dim Angle As System.Double Dim ArrowSize As System.Double Dim Text As System.String Dim TextHeight As System.Double Dim WitnessGap As System.Double Dim WitnessOvershoot As System.Double Dim value As System.Boolean   value = instance.CreateOrdinateDim(P0, P1, P2, P3, P4, Angle, ArrowSize, Text, TextHeight, WitnessGap, WitnessOvershoot) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateOrdinateDim(     System.object P0,    System.object P1,    System.object P2,    System.object P3,    System.object P4,    System.double Angle,    System.double ArrowSize,    System.string Text,    System.double TextHeight,    System.double WitnessGap,    System.double WitnessOvershoot ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateOrdinateDim(  &   System.Object^ P0, &   System.Object^ P1, &   System.Object^ P2, &   System.Object^ P3, &   System.Object^ P4, &   System.double Angle, &   System.double ArrowSize, &   System.String^ Text, &   System.double TextHeight, &   System.double WitnessGap, &   System.double WitnessOvershoot ) ``` | |

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

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateOrdinateDim.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)