<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IAddTrimmingLoop.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddTrimmingLoop Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : IAddTrimmingLoop Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CurveCount*

*Order*

*Dim*

*Periodic*

*NumKnots*

*NumCtrlPoints*

*Knots*

*CtrlPointDbls*

Obsolete. Superseded by [ISurface::IAddTrimmingLoop2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IAddTrimmingLoop2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IAddTrimmingLoop( _    ByVal CurveCount As System.Integer, _    ByRef Order As System.Integer, _    ByRef Dim As System.Integer, _    ByRef Periodic As System.Integer, _    ByRef NumKnots As System.Integer, _    ByRef NumCtrlPoints As System.Integer, _    ByRef Knots As System.Double, _    ByRef CtrlPointDbls As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim CurveCount As System.Integer Dim Order As System.Integer Dim Dim As System.Integer Dim Periodic As System.Integer Dim NumKnots As System.Integer Dim NumCtrlPoints As System.Integer Dim Knots As System.Double Dim CtrlPointDbls As System.Double   instance.IAddTrimmingLoop(CurveCount, Order, Dim, Periodic, NumKnots, NumCtrlPoints, Knots, CtrlPointDbls) ``` | |

| C# |  |
| --- | --- |
| ``` void IAddTrimmingLoop(     System.int CurveCount,    ref System.int Order,    ref System.int Dim,    ref System.int Periodic,    ref System.int NumKnots,    ref System.int NumCtrlPoints,    ref System.double Knots,    ref System.double CtrlPointDbls ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IAddTrimmingLoop(  &   System.int CurveCount, &   System.int% Order, &   System.int% Dim, &   System.int% Periodic, &   System.int% NumKnots, &   System.int% NumCtrlPoints, &   System.double% Knots, &   System.double% CtrlPointDbls ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CurveCount*

*Order*

*Dim*

*Periodic*

*NumKnots*

*NumCtrlPoints*

*Knots*

*CtrlPointDbls*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::IAddTrimmingLoop.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)